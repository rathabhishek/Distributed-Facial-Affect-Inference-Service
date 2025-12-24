# Security Policy

Reporting a vulnerability
- If you discover a security issue, please open a private report to the repository owner or use the project's designated security contact.

Secrets handling
- Never commit secrets, API keys, or private keys to the repository.
- Use environment variables or a secrets manager (AWS Secrets Manager, Azure Key Vault) for runtime secrets.

Repository hygiene
- Keep large datasets and trained models out of the repo. Use external storage (S3, Azure Blob) and reference them in documentation.
- Use `.gitignore` to exclude local environments, datasets, and keys.

CI/CD recommendations
- Add automated secret scanning to CI (e.g., detect-secrets, truffleHog) and enforce branch protection rules.

Encryption and access
- Use least-privilege IAM roles for cloud resources and rotate credentials regularly.

If you need assistance
- I can scaffold CI secret-scanning, IaC templates (Terraform/ARM/Bicep), or Kubernetes manifests and demonstrate secure secret integration.