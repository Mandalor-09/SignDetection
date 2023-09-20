# SignDetection
 Assistant
## YOLOv5 Object Detection with Custom Dataset

### Step 1: Create a Custom Dataset

1.  Collect images for each class you want to detect. In this example, we are creating a dataset for 6 classes: "Hello", "Yes", "No", "Thanks", "IloveYou", and "Please".
2.  Create a directory for the images and organize them into subdirectories for each class. For example:
```
data/
├── Hello
│   ├── Hello_1.jpg
│   ├── Hello_2.jpg
│   ├── Hello_3.jpg
├── Yes
│   ├── Yes_1.jpg
│   ├── Yes_2.jpg
│   ├── Yes_3.jpg
├── No
│   ├── No_1.jpg
│   ├── No_2.jpg
│   ├── No_3.jpg
├── Thanks
│   ├── Thanks_1.jpg
│   ├── Thanks_2.jpg
│   ├── Thanks_3.jpg
├── IloveYou
│   ├── IloveYou_1.jpg
│   ├── IloveYou_2.jpg
│   ├── IloveYou_3.jpg
├── Please
│   ├── Please_1.jpg
│   ├── Please_2.jpg
│   ├── Please_3.jpg
```

3.  Create a file named `labels.txt` and list the classes in the same order as the subdirectories. For example:
```
Hello
Yes
No
Thanks
IloveYou
Please
```

### Step 2: Train the Model

1.  Install the required dependencies:
```
pip install -r requirements.txt
```

2.  Download the YOLOv5 repository:
```
git clone https://github.com/ultralytics/yolov5
```

3.  Create a new directory for the training data:
```
mkdir data/train
```

4.  Copy the images from the custom dataset into the `train` directory:
```
cp -r data/Hello data/train/Hello
cp -r data/Yes data/train/Yes
cp -r data/No data/train/No
cp -r data/Thanks data/train/Thanks
cp -r data/IloveYou data/train/IloveYou
cp -r data/Please

5.  Models best weight is stored at location 'C:\Users\DELL\OneDrive\Desktop\SignDetection\yolov5s\yolov5s.pt'
