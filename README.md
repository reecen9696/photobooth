# photobooth

# Photobooth

Photobooth is a web application that allows users to take photos and post them to a public photo board. All uploaded photos are stored in an AWS S3 bucket and displayed on the website.

## Features

- 📸 Take photos and upload them
- 🖼️ View all uploaded photos on a public board
- 🗑️ Delete photos when needed
- 🚀 Hosted on AWS with Lambda functions handling uploads and deletions

## Tech Stack

- **Frontend:** React/Next.js (to be developed later)
- **Backend:** AWS Lambda (Node.js/Python)
- **Storage:** Amazon S3
- **Deployment:** AWS SAM + GitHub Actions

## Directory Structure

```
photobooth/
│── backend/                  # AWS Lambda + S3 logic
│   ├── upload-photo/          # Upload Lambda function
│   ├── delete-photo/          # Delete Lambda function
│   ├── package.json           # Backend dependencies
│── frontend/                  # React or Next.js frontend (later)
│── .github/workflows/         # GitHub Actions CI/CD
│── README.md                  # Project documentation
│── .gitignore                 # Ignore files we don’t want in GitHub
```

## Getting Started

### 1️⃣ Clone the Repository

```bash
git clone git@github.com:reecen9696/photobooth.git
cd photobooth
```

### 2️⃣ Set Up AWS Credentials

Ensure you have AWS CLI installed and configured:

```bash
aws configure
```

Grant necessary permissions for Lambda to access S3.

### 3️⃣ Deploy Backend with AWS SAM (to be added)

```bash
sam build
sam deploy --guided
```

### 4️⃣ Run the Frontend (Coming Soon)

```bash
cd frontend
npm install
npm start
```

## Deployment

GitHub Actions will be used for automatic deployment of Lambda functions and frontend updates.

## Next Steps

- [ ] Implement AWS Lambda functions for upload & delete
- [ ] Set up API Gateway for frontend integration
- [ ] Develop the React-based frontend
- [ ] Automate deployment with GitHub Actions

---

**📌 Stay tuned for updates as we build Photobooth!** 🚀
