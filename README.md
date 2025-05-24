# Detecting-steganography-with-tools-like-StegExpose-analyzing-file-signatures
# Name: Kavi Keerthana R 
# Reg No: 212222100022
## AIM:
To detect hidden data using steganography detection tools like StegExpose and analyze file signatures for authenticity and manipulation.

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROCEDURE:
### Step 1: Download Image and Create Secret Message File
  •	Download a .jpeg image (e.g., praveen.jpeg) from a trusted website or use own image.
  
  ![image](https://github.com/user-attachments/assets/e9a2c6df-0395-4318-be4d-cc569e888235)

  •	Create a text file named secret with a confidential message:
  
  ![image](https://github.com/user-attachments/assets/aa38483f-95fa-4bdc-9d69-25c0e53f71c0)


### Step 2: Install and Verify Steghide Tool
  •	Install Steghide on Kali linux and confirm the installation by checking its version:
  
![image](https://github.com/user-attachments/assets/705969c0-79f2-4fb2-a589-909c0311eb3b)

 
### Step 3: Embed the Secret Message into the Image
  •	Use the following command to embed secret into praveen.jpeg:

  ![image](https://github.com/user-attachments/assets/0538b48e-5147-4a9f-b9b7-2d9c6b61ba98)


### Step 4: Delete the Original Secret File
  •	After embedding, delete the plaintext file:
  
  ![image](https://github.com/user-attachments/assets/24630a33-8710-4d42-a208-7bee7a8d3f90)


## OUTPUT:
### Step 1: Extract the Embedded Secret from the Image
  •	To retrieve the hidden file:
  
  ![image](https://github.com/user-attachments/assets/47598efe-c267-4e46-91d1-85da28e50ec4)


  •	Enter the same passphrase used during embedding.
  
  ![image](https://github.com/user-attachments/assets/6953f7d2-4abc-4106-8463-2473db0f713f)



### Step 2: Verify the Extracted Message

  •	Display the extracted file content to verify:
  
  •	Ensure the message matches the original secret content.

  •	Another command to see the same secret message is
  
  ![image](https://github.com/user-attachments/assets/d9056985-6c34-4c09-b36f-50709cb90886)


 
### Step 3: Retrieve Information About the Embedded Data
  •	To gather details about embedded content in the image:
  
  ![image](https://github.com/user-attachments/assets/9520c726-821a-4b83-95de-8272e54bde5e)
 
  
  •	This will display file type, size, and whether data is embedded.


## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
