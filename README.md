
# IMPORTANT NOTICE: 
The model is too large to store on github (165 mb), download it from this gdrive [link](https://drive.google.com/file/d/1gt0WlQmDNakDTlcrvcE-3LFMi9BP1ZCE/view?usp=drive_link) and move it into the base directory instead. I am working on a way to deal with the issue.

# KKP Blood Screening Project

## Description
The KKP Blood Screening Project is a web application designed for blood analysis using YOLOv5 object detection model deployed with Flask. This application allows users to upload an image and receive a labeled result indicating various blood cell types. The model is trained to detect 11 classes of blood cells, including:
- Lymphoblast: 752 instances
- Neutrophil: 263 instances
- Promyelocytes: 137 instances
- Dysplastic_Cell: 6 instances
- Lymphocytes: 4 instances
- Myelocytes: 4 instances
- Band_Neutrophils: 2 instances
- Nucleated_RBC: 2 instances
- Giant_Platelet: 1 instance
- Monocytes: 1 instance

For more detailed information about these cell types, refer to the `blood_detect` folder.

## Installation and Setup
To run the project locally for development purposes, follow these steps:
1. Create a virtual environment:
   ```bash
   python3 -m venv venv
   ```
2. Activate the virtual environment:
   ```bash
   source venv/bin/activate
   ```
3. Install the required dependencies:
   ```bash
   (venv) $ pip install -r requirements.txt
   ```
4. Run the Flask web application:
   ```bash
   (venv) $ python webapp.py
   ```

Additionally, an example Python script for performing inference using requests is provided in `tests/test_request.py`. Please note that the `find_model()` function within this script expects a file ending with `.pt` for inference, and the code will work only if there is one model file ending with `.pt` placed inside the folder. Adjust the script accordingly if multiple model files are present.

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgments
- This project utilizes the YOLOv5 model developed by Ultralytics.
