# Detecting-steganography-with-tools-like-StegExpose-analyzing-file-signatures
## AIM:
To detect hidden data using steganography detection tools like StegExpose and analyze file signatures for authenticity and manipulation.

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROGRAM:
StegExpose and File Signature Analysis Commands

## OUTPUT:
- **1.Install and Set Up StegExpose**
• Download the StegExpose .jar file from the official repository.
• Ensure Java Runtime Environment (JRE) is installed.
• Run the tool on an image or a folder of images:\

• The output will list detection scores and a "suspect" verdict if steganography
is found.

- **2.Scan Individual Files**
• Run StegExpose on a single image:

The tool uses statistical analysis methods like RS analysis, Sample Pair
analysis, and Chi-square attack to detect hidden content.

- **3.Analyze File Signatures**
• Use Linux commands to verify the file's true format:

Every file type has a magic number (e.g., JPEG files start with FFD8). Comparing
the actual signature with the file extension helps identify mismatches or embedded
file tricks.

- **4. Cross-Check File Behavior**
• Rename the file (e.g., mv suspicious.jpg suspicious.zip) and try extracting it:

o Sometimes, files are disguised (e.g., a ZIP file hidden as a JPG), and this
trick helps uncover such embedded archives.

- **5.Optional: Use Other Tools**

o Tools like binwalk, stegsolve, or zsteg can be used for deeper analysis,
especially for PNG files or binary dumps.

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/e3c17886-4b2d-49cf-a1d1-44c2b4269274" />

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/0969ecc8-d17e-477b-a879-d2a4d39b9279" />



<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/6a33cc39-ea21-4ed9-87f9-1005820d46d6" />


<img width="1914" height="479" alt="image" src="https://github.com/user-attachments/assets/a203d0ef-48d6-4e12-a17b-9f8595543857" />



<img width="1919" height="1074" alt="image" src="https://github.com/user-attachments/assets/48c61a51-f41f-4a6a-b167-9018979aa4b6" />



## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
