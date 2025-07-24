## 🧱 Architecture
```mermaid
flowchart TD
    A[Developer] -->|Push Code| B[GitHub]
    B -->|Triggers| C[AWS CodePipeline]
    C -->|Deploy to| D[S3 Staging Bucket]
    D -->|Manual Approval| E[S3 Production Bucket]
    E --> F[CloudFront CDN]
    F --> G[End Users]
    H[Route 53] --> F
    I[ACM SSL] --> F
