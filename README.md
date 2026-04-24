# 😎 Sunglass Filter using OpenCV

##  Project Overview
This project demonstrates how to overlay a sunglass image onto a human face using image processing techniques in Python. It uses alpha blending and masking to seamlessly place sunglasses over the eye region.

Built using **:contentReference[oaicite:0]{index=0}**, NumPy, and Matplotlib.

---

##  Objectives
- Read and display images
- Work with alpha channels (transparency)
- Resize and align overlay images
- Apply masking and blending techniques
- Generate a realistic augmented image

---

##  Technologies Used
- Python
- :contentReference[oaicite:1]{index=1}
- NumPy
- Matplotlib
- Jupyter Notebook

---

##  Project Structure
```
├── main_sunglass.ipynb # Main notebook
├── passport.JPG # Input face image
├── sunglass.png # Sunglass image (with alpha channel)
└── README.md
```
##  Output

###  Step 1: Original Face Image  
<img width="532" height="604" alt="image" src="https://github.com/user-attachments/assets/19f68ed9-1ffd-4647-a530-855dfd1bfcd7" />
 

###  Step 2: Sunglass Image  
<img width="1600" height="800" alt="sunglass" src="https://github.com/user-attachments/assets/46535d8b-77ce-4623-8ed9-9e5e890a40db" />


###  Step 3: Mask Visualization  
<img width="1389" height="211" alt="image" src="https://github.com/user-attachments/assets/beae604f-32e3-4471-894e-89761374d2ec" />


###  Step 4: Naive Output  
<img width="559" height="584" alt="image" src="https://github.com/user-attachments/assets/493827bf-517a-4de7-8333-96035525d867" />
 

###  Step 5: Final Output (Blended)  
<img width="1379" height="768" alt="image" src="https://github.com/user-attachments/assets/a8da9a48-7d89-461f-9357-57ae6edc8fbb" />


##  How It Works

### 1. Load Images
- Face image is loaded using OpenCV
- Sunglass image is loaded with alpha channel

### 2. Resize Sunglasses
- Adjust dimensions to match the eye region

### 3. Extract Channels
- Separate:
  - RGB (color channels)
  - Alpha (mask)

### 4. Create Mask
- Convert alpha channel into 3-channel mask

### 5. Overlay Sunglasses
Two approaches:
- **Naive overlay** (direct replacement)
- **Mask-based blending** (smooth and realistic)

##  Key Concepts

- Image slicing (Region of Interest - ROI)
- Alpha blending
- Bitwise operations
- Mask creation
- Channel separation
