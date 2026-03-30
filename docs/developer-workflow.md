# Developer Workflow

## Golden Path Workflow
1. Developer updates application code
2. CI pipeline runs code, dependency, container, and IaC checks
3. Image is built and scanned
4. Kubernetes manifests and policies are validated
5. Deployment proceeds only if controls are satisfied

## Engineering Goal
Enable developers to ship faster while inheriting secure defaults from the platform.