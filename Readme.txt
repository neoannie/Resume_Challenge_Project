# Resume Challenge Project  

Welcome to my Resume Challenge Project repository! This project showcases not only my resume but also acts as a full portfolio deployment built with AWS. It highlights my hands-on experience in setting up a static website with a fully automated 2-stage CI/CD pipeline.  

## 🚀 Project Overview  
This project deploys a static website hosted on Amazon S3, triggered by code commits pushed to GitHub. It uses a 2-stage CI/CD pipeline to deploy first to a staging environment and then to production. This setup demonstrates my DevOps and cloud engineering skills.  

## ✅ Key AWS Services Used:  
- **Amazon S3**: Static website hosting  
- **GitHub**: Source code and version control  
- **AWS CodePipeline**: CI/CD orchestration  
- **Amazon CloudFront**: Content delivery network (CDN)  
- **Amazon Route 53**: DNS management  
- **AWS Certificate Manager (ACM)**: SSL/TLS certificates  

## 🧱 Architecture  
![Architecture Diagram](portfolio.diagram.png)  

## 🔧 Services Breakdown  
- **S3**: Hosts static website files (HTML, CSS, JS)  
- **CodePipeline**:  
  - Source Stage: Pulls source from GitHub  
  - Deploy Stage: Deploys files to S3  
- **CloudFront**: Speeds up content delivery  
- **Route 53**: Manages custom domain DNS  
- **ACM**: Enables HTTPS via SSL/TLS  

## ⚙️ CI/CD Pipeline  
1. **Staging Stage**  
   - Deploys the latest code to a staging environment  
   - Used for testing and review  

2. **Production Stage**  
   - Deploys tested changes from staging to production  

## 🛠️ Setup Instructions  
### Prerequisites  
- AWS Account with IAM permissions  
- Registered domain name (e.g., from Route 53 or another provider)  
- Basic knowledge of AWS & GitHub  

### Steps to Set Up  
1. **Clone the repository**  
   ```bash
   git clone https://github.com/anniesingsit/resume-challenge
