# EEE1007
Image Denoising Using AutoEncoders
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
   
