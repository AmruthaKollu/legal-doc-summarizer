# Legal Document Summarization and Key Points Extraction System

## Overview
The Legal Document Summarization and Key Points Extraction System is an expert system designed to assist users in analyzing legal documents efficiently. Using NLP techniques and inference rules, the system automatically summarizes uploaded legal documents and highlights key clauses, such as confidentiality, termination, and payment terms.

---

## Features
- **Legal Document Upload**: Supports various formats (PDF, DOCX).
- **Automated Summarization**: Provides concise summaries of lengthy legal documents.
- **Key Clause Extraction**: Highlights essential clauses using rule-based inference.
- **User-Friendly Interface**: Built with Angular for seamless navigation.
- **Secure Storage**: Documents are securely managed using a MongoDB backend.

---

## System Architecture
![System Architecture](./path_to_architecture_image.png)

---

## Technologies Used

### **Frontend**
- Angular
- TypeScript

### **Backend**
- Node.js
- Express.js

### **Database**
- MongoDB

### **NLP Model**
- Pretrained NLP models like BERT or GPT for summarization and key clause extraction.

---

## Installation and Setup

### **Prerequisites**
1. Install [Node.js](https://nodejs.org/).
2. Install [MongoDB](https://www.mongodb.com/try/download/community).
3. Install Angular CLI:
   ```bash
   npm install -g @angular/cli
   ```

### **Steps**

#### **Backend Setup**
1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Configure environment variables in `.env` file:
   ```env
   PORT=3000
   MONGO_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/<dbname>
   JWT_SECRET=your_secret_key
   ```
4. Start the backend server:
   ```bash
   npm start
   ```

#### **Frontend Setup**
1. Navigate to the `frontend` directory:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Configure the API URL in `src/environments/environment.ts`:
   ```typescript
   export const environment = {
     production: false,
     apiUrl: 'http://localhost:3000' // Ensure this matches the backend URL
   };
   ```
4. Start the frontend server:
   ```bash
   ng serve
   ```

---

## Usage
1. Open the frontend in your browser at `http://localhost:4200`.
2. Upload a legal document in the supported formats.
3. View the generated summary and key points.

---

## Contribution
We welcome contributions to improve the system. Follow these steps:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit changes and push:
   ```bash
   git add .
   git commit -m "Add feature-name"
   git push origin feature-name
   ```
4. Create a pull request.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact
For any questions or feedback, feel free to contact the development team.
