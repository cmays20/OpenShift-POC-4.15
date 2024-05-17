# Install GitLab on OpenShift using GitOps

## Prerequisites

A secret is required to store you smtp password for emails to work.
```bash
oc create secret generic smtp-password \
  --from-literal=password=<YOUR_SMTP_PASSWORD>
```
NOTE: If you are using gmail, this will be an Application Password: https://myaccount.google.com/u/1/apppasswords