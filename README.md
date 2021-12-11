# EEE1007
Image Denoising Using AutoEncoders

For the enhancement of images and the extraction of relevant information from them, image processing techniques are widely utilised in the fields of sciences and computer vision. The elimination of various types of noise from images is a crucial step in image processing. During the storage, transmission, or acquisition of photographs, noise might appear in the image.If a model achieves both picture preservation and noise removal, it is considered a satisfactory de-noising model. Gaussian, salt and pepper, Speckle, and other types of noise can be found in an image. A model that can denoise several types of noises is seen to be superior to others.In this paper, we provide an autoencoder-based model for removing various types of noise from pictures. We used Gaussian noise, loss function MSE data, Optimize Adam to denoise the images.

## Contributors:
> Moudipa Jana - https://github.com/Moudipa01

> Deshansh Panchbhai - https://github.com/deshansh27/deshansh27

> S.Annapurna Shobitha - https://github.com/annapurna2003

## Getting Started:
Google Collab has a simple interface and it's very easy to import database in it's backend.

### Import kaggle environment in google collab:
    (1) Download the Kaggle API token.

     Go to “Account”, go down the page, and find the “API” section.
     Click the “Create New API Token” button.
     The “kaggle.json” file will be downloaded.
   
   (2) Mount the Google drive to the Colab notebook. 
   It means giving access to the files in your google drive to Colab notebook.
   
```python
   from google.colab import drive
drive.mount("/content/gdrive", force_remount=True)
```
   (3)  Install Kaggle API.
   
```python
! pip install -q kaggle
```
   (4)  Change the current working directory to where you want to download the Kaggle dataset.
   
```python
from google.colab import files
files.upload()
```
   
   (5) create a kaggle folder
```python
! mkdir ~/.kaggle
```
 (6) copy the kaggle.json to folder created
```python
! cp kaggle.json ~/.kaggle/
```

 (7) permison for the json to act
 ```python
 ! chmod 600 ~/.kaggle/kaggle.json
 ```
 
 (8) to list all datasets in kaggle
 ```python
! kaggle datasets list
```

 (9) download cat-and-dog database
 ```python
 !kaggle datasets download -d tongpython/cat-and-dog
 ```
 (10) unzip the folders to get the required dataset
 ```python
 !unzip cat-and-dog.zip
 ```
 
 ## Output:
 ### Original Image:
 ![image](https://user-images.githubusercontent.com/74910213/145670922-29bbc5c4-0809-43b4-9585-4693cce14e9c.png)

### Recontructed Image:
![image](https://user-images.githubusercontent.com/74910213/145670954-79c22a6e-d7f5-4c51-bc1f-fe65dd99cc64.png)

## The Accuracy of Project: 
![image](https://user-images.githubusercontent.com/74910213/145670994-704d347a-cfb4-4053-bb1c-93dd09534ae6.png)

 

   
