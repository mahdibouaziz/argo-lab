# argo-lab

# Argo CD Notification API Documentation

This API allows users to manage Argo CD notification credentials and templates per instance.

# Workflow Overview

To enable notifications on an Argo CD-managed application, users must follow these steps:

**1. Create Notification Credentials**

Use the POST /notifications/credentials endpoint to define credentials for GitHub, Email, or Microsoft Teams.

**2. Create Notification Templates**

Use the POST /notifications/templates endpoint to define how notifications should be sent.

⚠️ Templates cannot be created before credentials.

**3. Annotate Your Argo CD Application**

Update your Argo CD Application with the proper annotations to enable the notifications based on the configured triggers/templates.

# API Endpoints

