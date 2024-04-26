****Insect Detection Web Application************
This web-based application utilizes YOLOv5 for insect detection. It provides a user-friendly interface for users to upload images and detect insect pests in them. 
******General Dependenices******
****Installation****
Follow these steps to install and run the application:
**Clone This Repository:**
git clone https://github.com/anambibi/Insect_pest_detection.git
 and unzip yolov5_full code.zip folder

If you wish to train the YOLOv5 model yourself, follow these steps:
**Prepare Dataset:**
YOLOv5 models must be trained on labelled data in order to learn classes of objects in that data. Organize your dataset into yolo format using Roboflow.
**Train Model:**
python train.py --data data.yaml --cfg models/yolov5s.yaml --weights '' --batch-size 16 --epochs 150
**Evaluate Model:**
python val.py --data data.yaml --weights runs/train/exp/weights/best.pt
