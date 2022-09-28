# YOLOv7 Instance Segmentation.

Implementation of "YOLOv7: Trainable bag-of-freebies sets new state-of-the-art for real-time object detectors" Instance Segmentation.

- This implimentation is based on [yolov5](https://github.com/ultralytics/yolov5).
- Download Weights from [yolov7-seg.pt](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7-seg.pt)
- Create a virtual environment if necessary to avoid disturbing existing packages in your system.

# Creating vitrual environment

```
#For Windows users:
python3 -m venv yolov7segmentation
cd yolov7segmentation/Scripts
activate
cd ..
cd ..
```
```
#For Linux users:
python3 -m venv yolov7segmentation
source yolov7segmentation/bin/activate
```
## Usage : 
- Step 1: Clone the repository
```
git clone https://github.com/vidhyadharan-k/YOLOv7-Semantic-Segmentation.git
```
- Step 2: Move into segment directory:
```
cd segment
```
- Step 3: Install requirements:
```
pip install -r requirements.txt 
```
- Step 4: Use predict.py to obtain instance segmentation output on the inference. Enter the path of your video in the place of videopath.mp4
```
python predict.py --weights yolov7-seg.pt --source "videopath.mp4"
```
- Step 5: To detect specific classes use --classes attribute and give the class number (coco) as input arguement.
```
python predict.py --weights yolov7-seg.pt --source "videopath.mp4" --classes 2 
```
(for detecting and segmenting cars)


# Example :
![desk](https://user-images.githubusercontent.com/62550691/192598829-3b5e6c7b-9b4c-4812-8987-c76e50a90328.jpg)


# References :

- [Official YOLOv7 Instance segmentation.](https://github.com/WongKinYiu/yolov7/tree/u7)
- [YOLOv7 Segmentation + Tracking](https://github.com/RizwanMunawar/yolov7-segmentation)
