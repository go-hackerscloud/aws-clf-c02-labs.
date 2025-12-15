# Objective: Understand guardrails, budgets, and best practices to avoid surprises in cloud spend.

## Prerequisites: Access to AWS Billing or the root/IAM user from Lab 1

### Steps:

1. Set a Billing Alarm:
  Open CloudWatch → Alarms → Create Alarm
  Select a metric like "EstimatedCharges" or create a custom metric if necessary
  Set a threshold (e.g., alert if projected charges exceed $5)
2. Create a Budget:
  Open Billing → Budgets → Create a budget
  Set monthly budget (e.g., $5) and alert recipients
3. Enable Cost Explorer (optional) to view cost trends.
4. Take a quick tour of IAM best practices:
  Use MFA on root account
  Do not use root for daily tasks
  Use least privilege on IAM policies
5. Clean up resources created during labs to avoid charges (terminate EC2, delete S3 objects/buckets, remove unused IAM users).

## Expected Results:

Alerts and budgets configured to prevent unexpected costs.
Awareness of security best practices and governance.

## Assessment / Checklist:

1. Billing alert created
2. Budget configured with alerts
3. Resources cleaned up after labs
