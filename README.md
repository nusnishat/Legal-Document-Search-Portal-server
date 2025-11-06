# 📄 Legal Document Search API

A simple **Express.js** backend that allows searching through a collection of legal documentse.  
This API filters documents based on keywords in their **title**, **summary**, or **type**, and returns relevant results.

## 🚀 Features

- 🔍 **Search API** – Query documents by keywords.  
- 🧾 **Preloaded Legal Documents** – Includes example legal documents with titles, summaries, and creation dates.  
- ⚡ **Fast & Lightweight** – Built with Node.js and Express.js.  
- 🌐 **CORS Enabled** – Can be accessed easily from frontend clients.  

## 🛠️ Tech Stack

- **Node.js**
- **Express.js**
- **CORS**
- **Body-Parser**

## 📂 Project Structure
project-root/
├── server.js # Main Express server file
├── package.json
└── README.md

## ⚙️ Installation & Setup
### 1. Clone the repository
### 2. Install dependencies
npm install
### 3. Run the server
node server.js

### The server will start at:
http://localhost:8000

## 📡 API Endpoint
GET /search

Searches for legal documents matching the query.
### Request:
GET /search?query=agreement
### Response (200 OK):
[
  {
  "id": "1",
    "title": "Non-Disclosure Agreement (NDA)",
    "type": "NDA",
    "summary": "This Non-Disclosure Agreement (\"Agreement\") is entered into...",
    "dateCreated": "2024-01-15"
  }
]

### Error Responses:
Status	Message <br/>
400	{ "error": "Query is required" }  <br/>
404	{ "error": "No documents found" }

## Dependencies
Package	Purpose  <br/>
express	Web framework  <br/>
cors	Enables Cross-Origin Resource Sharing  <br/>
body-parser	Parses JSON request bodies <br/>

## Live url
https://legal-document-search-portal-server.onrender.com
