# Resume Challenge Project

Welcome to my Resume Challenge Project repository! This project showcases more than my resume—it’s my portfolio. It displays my skills and experience in setting up a static website using AWS services, including a two-stage CI/CD pipeline.

## Project Overview

This project sets up a CI/CD pipeline to automatically deploy a static website to an Amazon S3 bucket. The source code is hosted in my GitHub repository. Services used include:

- **S3 Bucket**: To store and host the static files.
- **GitHub**: As the version control system.
- **AWS CodePipeline**: To automate the CI/CD process.
- **CloudFront**: For content delivery.
- **Route 53**: For DNS management.
- **ACM**: For SSL/TLS certificates.

## Architecture

![Architecture](architecture.png)

## CI/CD Pipeline

- **Staging**: Deploys to a test environment.
- **Production**: Deploys to the live environment after testing.

## Setup Instructions

1. Clone the repository.
2. Create an S3 bucket and upload your website files.
3. Set up AWS CodePipeline with GitHub integration.
4. Configure CloudFront for global content delivery.
5. Use Route 53 to manage domain settings.
6. Use ACM for HTTPS/SSL.
7. Push your code to GitHub — CodePipeline handles the rest!

## Production URL

[https://singsit.azzyalfie.com](https://singsit.azzyalfie.com)

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
