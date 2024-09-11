# Project Title: Uploading File Directly via Frontend

---

## Project Details:
- **Project Demo URL:** [https://directupload.redbeach-1a952c62.centralindia.azurecontainerapps.io/]
- **Demo Video URL:** [https://drive.google.com/file/d/1DA3_7_ZE8QHFLqU7I3RC4jfhniAPsQPs/view?usp=drive_link]
- **GitHub Repository URL:** [https://github.com/Prasad-b-git/direct-upload-to-azure-blob-storage]
- **Industry:** Technology

---

## Project Overview:
This project enables users to upload files directly from the frontend to Azure Blob Storage using a web interface. The project is deployed using Azure Container Registry and Azure Container Apps, providing a streamlined, scalable solution for direct file uploads.

---

## Technologies Used:
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Node.js (Express)
- **Azure Services:**
  - Azure Blob Storage: For storing uploaded files.
  - Azure Container Registry: For container image management.
  - Azure Container Apps: For containerized application deployment.
- **Other Libraries:**
  - Multer: Middleware for handling multipart/form-data, used for file uploads.
  - Azure Storage Blob SDK: For interactions with Azure Blob Storage.
  - OpenCV (Optional for Image Processing): Handles image manipulations, if needed.

---

## Key Features:

### **Direct File Upload via Frontend:**
- A user-friendly interface allowing drag-and-drop or browsing files for upload.
- Real-time feedback and display of uploaded files using JavaScript.
- Files are uploaded directly to Azure Blob Storage.

Screenshots of the file upload interface:

1. **With files present:**

![Uploaded Files](sandbox:/mnt/data/file-2cwcKLR206INleOktH030w3D)

2. **No objects in the bucket:**

![No Objects](sandbox:/mnt/data/file-XrO0PBBuWDcIelH1ZSo2BLJa)

---

### **SAS URL for Secure Uploads:**
- Secure Access Signature (SAS) URLs are generated on the server, allowing secure, time-limited file uploads to Azure Blob Storage.

---

### **Listing Uploaded Files:**
- After upload, users can view the list of uploaded files, which are fetched directly from the Azure Blob container.

---

## Deployment on Azure Container Apps:

### **Azure Services Used:**
- **Azure Blob Storage:** Manages files uploaded via the frontend, providing secure, scalable cloud storage.
- **Azure Container Registry (ACR):** Hosts the container image used for deployment. The Docker container is built and pushed to ACR, ensuring a streamlined deployment process.
- **Azure Container Apps:** Used for deploying and running the containerized application. It allows for a managed serverless environment that auto-scales based on traffic and resource needs.

---

## Future Enhancements:

### **Image Processing (Optional):**
- Integrate OpenCV for preprocessing or resizing uploaded images before storage.

### **Enhanced Security:**
- Implement more granular role-based access controls (RBAC) and fine-tuned permissions for file uploads and access.

### **File Metadata Management:**
- Include functionality to store metadata such as upload timestamp, file size, etc., in Azure SQL or a similar database.

---

## Deployment Process:

1. **Building Docker Image:** A Dockerfile is used to containerize the application. The image is pushed to Azure Container Registry.
2. **Deploying with Azure Container Apps:** The containerized application is deployed using Azure Container Apps, providing scalability and integration with other Azure services.

---

