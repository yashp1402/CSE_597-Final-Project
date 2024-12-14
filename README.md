# CSE_597-Final_Project
### Name - Yash Priyadarshi
### PSU ID - yvp5218

Paper Replication for **Composed Image Retrieval using Contrastive Learning and Task-oriented CLIP-based Features**. <br/>
Paper Link - https://arxiv.org/abs/2308.11485

### Start with cloning th emain repository
git clone https://github.com/ABaldrati/CLIP4Cir

### Install the following dependencies
`pip install comet-ml` <br/>
`pip install git+https://github.com/openai/CLIP.git`

### Downloading the fashionIQ dataset
Use below drive link to download the fashionIQ dataset. <br/>
https://drive.google.com/file/d/18lDDTXGxiw6JFLf6b9j4kQIaZsyJOBQP/view?usp=sharing

### Preprocessing
Use the `resize_images.py` script to resize the images as per the paper requirements. <br/>
For RN50 we need `224 x 224` and for RN50 we neeed `288 x 288`. 
We can do this by the following command
`python resize_images.py  --image_dir IMAGE_DIR --output_dir OUTPUT_DIR --image_size IMAGE_SIZE`

We also need to copy the pretrained weights in the CLIP4Cir irectory.
The parent directory has to follow the following structure in order for the scripts to work.

<img width="260" alt="Screenshot 2024-12-12 at 8 38 36 PM" src="https://github.com/user-attachments/assets/17b47827-be67-4e12-a05a-9066c9378747" />


### Training and Validation
For this just follow the uploaded file Paper_Implementation.ipynb. Just make sure to place this file in the CLIP4Cir directory or set the same as the current work directory.
