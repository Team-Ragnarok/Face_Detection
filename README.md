## Face_Detection
**Project for IITSoC**

This project performs Multi-person face detection using MTCNN, while the main model is trained using Siamese Network(Facenet).  
The front-end is developed from Flask WebApp.  

***Steps to run:***  
1. Install dependencies from `requirements_cpu` or `requirements_gpu` using the following code:  
    ```bash
    pip install -r requirements_cpu.txt
    ```
    or 
    ```bash
    pip install -r requirements_gpu.txt
    ```
   *Note*: If you have a NVIDIA GPU, you must first install the CUDA libraries.  
   *Note*: It is advised to create this project on a python virtual environment(Link-https://docs.python.org/3/tutorial/venv.html).  
    
2. Install the pre-trained model from the link-https://drive.google.com/file/d/0B5MzpY9kBtDVZ2RpVDYwWmxoSUk/edit.  
   Place this model under the model folder such that the path of the model corresponds as:  
   `../model/20170512-110547/20170512-110547.pb`
  
3. Run the flask server with the following code:
   ```bash
   python server.py
   ```
   The server is set up on default URL:`localhost:5000`  
   
4. Upload your images using the app interface(**.png**,**.jpeg**,**.jpg** only allowed). Make sure to name the image file as the name of the person inside the image.
   *Note*:When the image file is uploaded successfully, the cropped face images will appear in the `uploads/` folder, and the corresponding embedding files will appear in the
   `embeddings/` folder.

5. Click on `Click here for live facial recognition with Web Camera!` button to start the webcam feed. Press **q** from keyboard to take the image and close the webcam feed.  

6. Voilà, you'll get the all the present individuals displayed right on the image taken from Webcam.

***References***:
Facenet and MTCNN model source:"https://github.com/davidsandberg/facenet"

***Team:***
Aryan Rastogi    
Ashish Gautam     
Aditya Bharadwaj   
Bharat Gupta   
Vardhan Paliwal    
Purnadip Chakrabarti   

**This project was created for IITISoC 2020.**


