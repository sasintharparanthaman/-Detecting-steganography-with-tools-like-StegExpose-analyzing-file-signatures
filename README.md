# EXP8:DETECTING STEGANOGRAPHY WITH TOOLS  LIKE STEGEXPOSE,ANALYSING FILE SIGNATURES

## AIM:
To hide and extract secret information (e.g., text files) inside a cover file (e.g., JPEG image) using the steganography tool `steghide` in Kali Linux.

EQUIPMENTS REQUIRED:

●	Hardware: PCs

```
Register Number: 212223230199
Name: SASINTHAR P

```

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROCEDURE:
### Step 1: Download Image and Create Secret Message File
  •	Download a .jpeg image (e.g., nature.jpeg) from a trusted website or use own image.
  
![Screenshot 2025-04-26 103140](https://github.com/user-attachments/assets/287cced8-e919-49a1-a328-4ff316cee5fb)


  
  •	Create a text file named secret with a confidential message:
  



### Step 2: Install and Verify Steghide Tool
  •	To install Steghide on Kali linux,run:
  
  ![Screenshot 2025-04-26 104503](https://github.com/user-attachments/assets/4c9fcf64-e42d-499e-9af5-301a75e6ffb5)

  •	Confirm the installation by checking its version:
  
 
![Screenshot 2025-04-26 104539](https://github.com/user-attachments/assets/d8cdc76b-2e23-463c-af76-2b9be2627e3e)

 
### Step 3: Embed the Secret Message into the Image
  •	Use the following command to embed secret into nature.jpeg:
  
![Screenshot 2025-04-26 105313](https://github.com/user-attachments/assets/c6ec22ef-25a6-4c85-8193-5884208efbb3)



### Step 4: Delete the Original Secret File
  •	After embedding, delete the plaintext file:
  
![Screenshot 2025-04-26 105414](https://github.com/user-attachments/assets/ff080f61-d2b2-488d-a76b-834f22c7d319)


## OUTPUT:
### Step 1: Extract the Embedded Secret from the Image
  •	To retrieve the hidden file:

![Screenshot 2025-04-26 105608](https://github.com/user-attachments/assets/2b4a6b5f-cd0f-40e6-b965-935d2d2a678a)

  •	Enter the same passphrase used during embedding.
  


### Step 2: Verify the Extracted Message

  •	Display the extracted file content to verify:
  
![Screenshot 2025-04-26 105726](https://github.com/user-attachments/assets/e3adacda-56e8-4a5e-90b0-42db916b6012)


  
  •	Ensure the message matches the original secret content.
  
  •	Another command to see the same secret message is
  

![Screenshot 2025-04-26 110324](https://github.com/user-attachments/assets/ba2b1bb8-119d-4eef-9109-355b1eebf5df)

 
### Step 3: Retrieve Information About the Embedded Data
  •	To gather details about embedded content in the image:
  
![Screenshot 2025-04-26 111536](https://github.com/user-attachments/assets/c0605a51-f985-4ba8-862c-6a4e40b68575)   

  •	This will display file type, size, and whether data is embedded.

 
## RESULT:
Embedded "secret" into praveen.jpeg successfully using Steghide with passphrase 12345.Extracted and verified hidden message
