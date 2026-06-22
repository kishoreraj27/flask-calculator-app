# Flask Calculator Application

A simple and responsive calculator web application built using **Flask** and containerized using **Docker**.

## Features

* Addition
* Subtraction
* Multiplication
* Division
* User-friendly interface
* Dockerized application
* Easy deployment on AWS EC2

## Technologies Used

* Python
* Flask
* HTML
* CSS
* Docker
* Git
* GitHub

## Project Structure

```text
flask-calculator-app/
│
├── app.py
├── Dockerfile
├── requirements.txt
├── .gitignore
├── README.md
│
└── templates/
    └── index.html
```

## Run Locally

### Clone the Repository

```bash
git clone https://github.com/<your-github-username>/flask-calculator-app.git
cd flask-calculator-app
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Start the Application

```bash
python app.py
```

### Access the Application

```text
http://localhost:5000
```

## Docker Setup

### Build Docker Image

```bash
docker build -t flask-calculator:v1 .
```

### Run Docker Container

```bash
docker run -d -p 5000:5000 --name flask-calculator flask-calculator:v1
```

### Verify Running Container

```bash
docker ps
```

### View Logs

```bash
docker logs flask-calculator
```

## AWS EC2 Deployment

1. Launch an Amazon Linux EC2 instance.
2. Install Docker.
3. Clone the repository.
4. Build the Docker image.
5. Run the container.
6. Allow HTTP traffic on port 80 in the Security Group.

Example:

```bash
git clone https://github.com/<your-github-username>/flask-calculator-app.git

cd flask-calculator-app

docker build -t flask-calculator:v1 .

docker run -d -p 80:5000 --name flask-calculator flask-calculator:v1
```

Access:

```text
http://<EC2-Public-IP>
```

## Future Enhancements

* Scientific Calculator
* Calculator History
* GitHub Actions CI/CD Pipeline
* Docker Hub Integration
* Automated AWS Deployment
* Terraform Infrastructure Provisioning

## Author

**Kishore Raj**

* GitHub: https://github.com/kishoreraj27
* LinkedIn: https://linkedin.com/in/kishoreraj2709
