# 📬 MailFlow API

A lightweight REST API built with FastAPI for handling and validating email requests.

MailFlow API provides a simple backend structure for receiving email data, including the sender, recipients, subject, and message body. It uses FastAPI and Pydantic to validate incoming requests and demonstrates the fundamentals of building a RESTful API.

> ⚠️ This project currently validates and processes email request data but does not yet send real emails.

## ✨ Features

* 🚀 FastAPI-powered REST API
* 📩 Email request handling
* 👤 Sender information
* 👥 Support for multiple recipients
* 📝 Email subject and body validation
* 🔍 Automatic request validation using Pydantic
* 📚 Interactive API documentation

## 🛠️ Tech Stack

* Python
* FastAPI
* Pydantic
* Uvicorn

## 📂 Project Structure

```text
mailflow-api/
│
├── api.py
├── README.md
└── requirements.txt
```

## ⚙️ API Endpoint

### Send Mail

**POST**

```text
/send-mail/
```

### Request Body

```json
{
  "sender": "sender@example.com",
  "recipients": [
    "recipient1@example.com",
    "recipient2@example.com"
  ],
  "subject": "Hello!",
  "body": "This is a test email."
}
```

### Response

```json
{
  "message": "Mail sent successfully"
}
```

## 🚀 Getting Started

### Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/mailflow-api.git
cd mailflow-api
```

### Install dependencies

```bash
pip install fastapi uvicorn
```

### Run the application

```bash
python api.py
```

The API will run at:

```text
http://localhost:8000
```

## 📚 Interactive API Documentation

FastAPI automatically provides interactive documentation.

After starting the application, visit:

```text
http://localhost:8000/docs
```

You can use the Swagger UI to explore and test the API directly from your browser.

## 🔮 Future Improvements

* [ ] Implement actual email delivery using SMTP
* [ ] Add email service integration
* [ ] Add authentication and authorization
* [ ] Add environment variables for sensitive configuration
* [ ] Add request logging
* [ ] Add error handling
* [ ] Add unit tests
* [ ] Add asynchronous email processing
* [ ] Containerize the application using Docker
* [ ] Deploy the API
