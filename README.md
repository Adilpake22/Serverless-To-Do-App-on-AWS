# 🚀 Serverless To-Do App on AWS

A simple and scalable serverless To-Do application built using AWS services. This project demonstrates how to create a full-stack application using AWS Lambda, API Gateway, and DynamoDB.

---

## 📌 Features

- ➕ Add new tasks
- 📋 View all tasks
- ☁️ Fully serverless architecture
- ⚡ Fast and scalable
- 🌐 REST API integration

---

## 🛠️ Tech Stack

| Layer    | Technology           |
|----------|----------------------|
| Frontend | HTML, CSS, JavaScript |
| Backend  | AWS Lambda           |
| API      | AWS API Gateway      |
| Database | AWS DynamoDB         |

---

## 🏗️ Architecture

```
User → Frontend (HTML/JS) → API Gateway → Lambda → DynamoDB
```

---

## 📷 Screenshots
<img width="1913" height="961" alt="image" src="https://github.com/user-attachments/assets/caa74074-592a-42d2-82ee-d2818dbf5f68" />
<img width="1897" height="795" alt="api gateway" src="https://github.com/user-attachments/assets/4bfb178d-da67-421b-8092-e7fef299f694" />


---

## ⚙️ Setup Instructions

### 1. Clone Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
```

### 2. Run Locally

```bash
cd your-repo-name
python -m http.server 8000
```

Open in browser:

```
http://localhost:8000
```

---

## 🔗 API Endpoint

> ⚠️ **Note:** The AWS backend for this project has been **deleted** to avoid cloud charges.
> The API endpoint below is **no longer active**.
> If you want to run this project, please deploy your own AWS resources (see setup guide below).

```
https://988r89akel.execute-api.ap-southeast-2.amazonaws.com/dev  ← (Inactive)
```

---

## ☁️ AWS Cleanup — Avoiding Unwanted Charges

> This section is for anyone who has deployed this project on AWS and wants to **shut it down to stop billing**.

After you're done with the project, delete the following AWS resources to avoid charges:

### 🗑️ Resources to Delete

| Service | Where to Find It | Action |
|---|---|---|
| **DynamoDB Table** | Console → DynamoDB → Tables | Select table → Delete |
| **Lambda Function** | Console → Lambda → Functions | Select function → Actions → Delete |
| **API Gateway** | Console → API Gateway | Select API → Actions → Delete |
| **CloudWatch Logs** | Console → CloudWatch → Log Groups | Delete `/aws/lambda/your-function-name` |

### 💡 Tips to Verify No Charges

1. Go to **AWS Console → Billing & Cost Management → Bills** and check for pending charges.
2. Check **Free Tier usage** — Lambda gives 1M requests/month free, DynamoDB gives 25GB free.
3. Set a **Billing Alert**: Budgets → Create Budget → Set a $0.01 alert to get notified by email.

### ⚠️ Important

- Always delete **API Gateway first** if your endpoint is public — anyone calling it can generate charges.
- Make sure you are in the **correct AWS region** (this project used `ap-southeast-2` — Sydney).
- After deleting, wait **24–48 hours** and recheck the Billing Dashboard to confirm $0 usage.

---

## 📚 What I Learned

- Building serverless applications using AWS
- Creating REST APIs with API Gateway
- Using DynamoDB for data storage
- Handling CORS issues
- Connecting frontend with backend APIs

---

## 🚀 Future Improvements

- ✏️ Update tasks
- ❌ Delete tasks
- 🎨 Improve UI/UX
- 🔐 Add authentication (AWS Cognito)

---

## 👨‍💻 Author

Aditya Dilpake

---

## ⭐ If you like this project

Give it a star on GitHub ⭐
