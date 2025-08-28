# OralVis_Task
Training Code:
!pip install ultralytics
from ultralytics import YOLO

weights_path = 'yolov8s.pt'  

model = YOLO(weights_path)


model.train(
    data='/content/dataset/data.yaml',
    epochs=100,         
    imgsz=640,          
    batch=16,           
)
