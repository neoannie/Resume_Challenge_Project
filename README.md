# 🌩️ Resume Challenge Project  

Welcome to my **Resume Challenge Project** repository!  
This project serves as both a **portfolio website deployment** and a demonstration of my **AWS and DevOps skills**.  
It highlights hands-on experience with **static website hosting**, **CI/CD automation**, and **cloud infrastructure management** using AWS services.  

---

## 🚀 Project Overview  

This project deploys a **static website hosted on Amazon S3**, automatically triggered by code commits pushed to **GitHub**.  
A **two-stage CI/CD pipeline** is implemented to deploy changes first to a **staging environment**, then to **production** — demonstrating real-world DevOps workflows for automation and reliability.  

---

## ✅ Key AWS Services Used  
- **Amazon S3** – Static website hosting  
- **GitHub** – Source code and version control  
- **AWS CodePipeline** – CI/CD orchestration  
- **Amazon CloudFront** – Content delivery network (CDN)  
- **Amazon Route 53** – DNS management  
- **AWS Certificate Manager (ACM)** – SSL/TLS certificates  

---

## 🧱 Architecture  

![Architecture Diagram](portfolio/diagram.png)  

### **Services Breakdown**
- **Amazon S3** – Hosts static website files (HTML, CSS, JS)  
- **AWS CodePipeline**  
  - **Source Stage:** Pulls source code from GitHub  
  - **Deploy Stage:** Uploads files to S3 for deployment  
- **Amazon CloudFront** – Speeds up global content delivery  
- **Amazon Route 53** – Manages custom domain and DNS records  
- **AWS Certificate Manager (ACM)** – Enables HTTPS and SSL/TLS encryption  

---

## ⚙️ CI/CD Pipeline  

**Stage 1: Staging**  
- Deploys the latest code to a staging S3 bucket  
- Used for testing and review  

**Stage 2: Production**  
- Deploys tested and approved changes from staging to production automatically  

---

## 🛠️ Setup Instructions  

### **Prerequisites**
- AWS account with required IAM permissions  
- Registered domain name (via Route 53 or another provider)  
- Basic knowledge of AWS and GitHub  

---

### **Deployment Steps**

1. **Clone the Repository**
   ```bash
   git clone https://github.com/anniesingsit/resume-challenge.git
   cd resume-challenge
   ```

2. **Create an S3 Bucket**
   - Go to **AWS Console → S3 → Create bucket**  
   - Enable **Static website hosting**  

3. **Set Up CodePipeline**
   - Go to **AWS Console → CodePipeline → Create pipeline**  
   - Connect to your **GitHub** repository  
   - Add a **Deploy stage** that uploads to the S3 bucket  

4. **Configure CloudFront**
   - Set S3 as the **origin**  
   - Configure caching and viewer settings  

5. **Set Up Route 53**
   - Create a **hosted zone**  
   - Add **DNS records** pointing to the CloudFront distribution  

6. **Request SSL/TLS Certificate via ACM**
   - Request a **public certificate**  
   - Validate it using **DNS validation** in Route 53  

7. **Deploy**
   - Push code changes to GitHub  
   - CodePipeline automatically detects changes and deploys to S3  

---

## 🌐 Live Demo  
**Production URL:**  
🔗 [https://singsit.azzyalfie.com](https://singsit.azzyalfie.com)  

---

## 🤝 Contributing  
Contributions are welcome!  
Feel free to fork this repository and submit a pull request.  
For major changes, please open an issue first to discuss your ideas.  

---

## 📄 License  
This project is licensed under the **MIT License**.  

---

💡 *This project demonstrates my practical knowledge of AWS services, CI/CD automation, and cloud-based web hosting. It is part of my journey to build scalable and secure DevOps solutions in real-world cloud environments.*  


