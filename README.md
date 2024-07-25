  ![download](https://github.com/user-attachments/assets/486278f1-6cef-42dd-a3bd-fd4ee9a9d73e)
<div align="center">
  <h1>Gesture Volume Control Using OpenCV and MediaPipe</h1>
 </div>
> This Project uses OpenCV and MediaPipe to Control system volume 

## 💾 REQUIREMENTS
+ opencv-python
+ mediapipe
+ comtypes
+ numpy
+ pycaw

```bash
pip install -r requirements.txt
```
***
### MEDIAPIPE
![mediapipe](https://github.com/user-attachments/assets/dd20a720-cb9f-4419-b25e-8f3b381e17b1)
<div align="center">
</div>
> MediaPipe offers open source cross-platform, customizable ML solutions for live and streaming media.

#### Hand Landmark Model
After the palm detection over the whole image our subsequent hand landmark model performs precise keypoint localization of 21 3D hand-knuckle coordinates inside the detected hand regions via regression, that is direct coordinate prediction. The model learns a consistent internal hand pose representation and is robust even to partially visible hands and self-occlusions.

To obtain ground truth data, we have manually annotated ~30K real-world images with 21 3D coordinates, as shown below (we take Z-value from image depth map, if it exists per corresponding coordinate). To better cover the possible hand poses and provide additional supervision on the nature of hand geometry, we also render a high-quality synthetic hand model over various backgrounds and map it to the corresponding 3D coordinates.<be>
