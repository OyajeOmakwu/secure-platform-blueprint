# Threat Model

## Scope
This threat model covers the sample application, CI/CD pipeline, container image flow, Kubernetes deployment, and Terraform-managed infrastructure patterns.

## Key Threats
- Privileged container execution
- Use of unsigned or untrusted images
- Deployment of vulnerable application artifacts
- Overly permissive IAM or Kubernetes RBAC
- Lateral movement due to weak network segmentation
- Credential leakage in CI/CD or source control

## Security Strategy
- Enforce workload restrictions through policy-as-code
- Fail builds on critical security findings
- Use non-root containers and image hygiene
- Standardize reusable secure infrastructure modules