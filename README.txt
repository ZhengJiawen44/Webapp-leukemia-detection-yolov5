Title: 
KKP Blood screening project (Yolov5 object detection model deployment using flask)




Description:
web app where you can upload an image and get back a labelled result.
the model consists of 11 classes:

Lymphoblast: 752 instances

Neutrophil: 263 instances

Promyelocytes: 137 instances

Dyplastic_Cell: 6 instances

Lymphocytes: 4 instances

myelocytes: 4  instances

Band_Neutrophils: 2  instances

nucleated_RBC: 2 instances

Giant_Platelet: 1 instances

monocytes: 1  instances
more addtional information about these cells can be found in the blood_detect folder.




installation and setup:
Run locally for dev, requirements mostly originate from yolov5:
python3 -m venv venv
source venv/bin/activate
(venv) $ pip install -r requirements.txt
and then run webapp.py

An example python script to perform inference using requests is given in tests/test_request.py
As the find_model() function will return a file ending with .pt for inferencing, the code only works when you have one model ending with .pt placed inside the folder.

