# Object Detection and Monitoring System for Indian Roads

1. Object Detection and Classification
2. Licence Plate and Trash Detection
3. Helmet Detection
4. Accident Detection
5. Getting Started - How to use it?



## 1. Object Detection and Classification

Using Ultralytics YOLOv8, the model was trained on 34 different classes specific to what's encountered on an Indian road. This is the main object detection system on an autonomous vehicle which runs on the dashcam, helping to reduce the number of accidents while driving and to safely navigate around in various traffic conditions.

https://github.com/Gacha76/HF24-KickBit/assets/114499152/eb56f7a1-22d7-4182-92ec-d2346d6b3914



## 2. Licence Plate and Trash Detection

Littering is a world-wide problem contributing to land pollution. To discourage and prevent further littering, a license plate and litter detection system is implemented which detects the licence plate of the littering vehicle and reads the number using OCR. This extracted number is then stored in the database along with the video frame snapshot which gets displayed on the Flask website. Further action can be taken by the authorities for the offending vehicle.

https://github.com/Gacha76/HF24-KickBit/assets/114499152/91f1af61-514a-4ce9-b974-699a2498188c



## 3. Helmet Detection

Safety is vital when driving. It's required that a driver needs to wear a helmet along with the passengers. The helmet detection system can detect whether a person is wearing a helmet or not and stores the snapshot along with the vehicle license plate number extracted using OCR which is displayed in the website in case any driver or passenger is found violating this rule.

https://github.com/Gacha76/HF24-KickBit/assets/114499152/c859aec9-3dd7-4750-967a-d6675b45ad89



## 4. Accident Detection

A CNN is trained to detect accidents via dashcam. As much as we try to prevent accidents from occuring, we have to be prepared when the event occurs. We can store the GPS coordinates along with a snapshot of the video frame in a database and the respective authorities will recieve an alert, prompting swift action and arrival of help in the least amount of time.

https://github.com/Gacha76/HF24-KickBit/assets/114499152/71161db9-50ba-41da-8d66-05330e82069b



## 5. Getting Started - How to use it?

### Setup

- Make sure `Tesseract` is installed on your system to perform OCR on the license plates
- Clone the repository `https://github.com/Gacha76/HF24-KickBit.git`
- Create a new environment using `Python 3.10.13`
- Install the dependencies `pip install -r requirements.txt`

### Running the code

- To run the accident detection system, run `main.py`
- To run the helmet detection system, run `run_helmet_detection.py`
- To run the litter detection system, run `litter_plate_detection.py`
- The flask websitecan be accessed by running `python flaskapp.py`
