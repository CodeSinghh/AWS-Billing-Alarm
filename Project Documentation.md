
A step-by-step guide to creating a billing alarm in AWS CloudWatch to monitor your account charges and receive alerts when they exceed a specified threshold.

## Step 1: Enable Billing Alerts

1. **Go to the AWS Billing Console:** Open [AWS Billing Console](https://console.aws.amazon.com/billing/).
   - Ensure you are in the **US East (N. Virginia)** region.
   - Sign in as a root user or an IAM user with permissions to view billing information.
   
2. **Enable Billing Alerts:**
   - Choose **Billing preferences**.
   - Check the box for **Receive Billing Alerts**.
   - Click **Save preferences**.

   > **Note:** After enabling billing alerts, it will take approximately 15 minutes before you can view the billing data and set billing alarms.

## Step 2: Create CloudWatch Billing Alarm

1. **Go to the CloudWatch Console:** Open [CloudWatch Console](https://console.aws.amazon.com/cloudwatch/).
   - Ensure you are in the **US East (N. Virginia)** region as all the billing metric data is stored in this region.

2. **Create an Alarm:**
   - Click on **All alarms** in the left navigation pane.
   - Click **Create alarm**.

3. **Select Metric:**
   - Click on **Select metric**.
   - Under the **All metrics** tab, choose **Billing**.
   - Under **Billing**, select **Total Estimated Charge**.

4. **Configure Metric:**
   - Select **metrics (USD)**.
   - Under **Graphed metrics**, click on **Select metric** at the bottom of the screen.

5. **Set Threshold Value:**
   - Enter a threshold value (e.g., 5 USD) or based on your requirement.

6. **Set Notification:**
   - Under **Notification**, either select an existing SNS topic or create a new topic.
   - Click **Next** at the bottom of the screen.

7. **Finalize Alarm:**
   - Give your alarm a meaningful name.
   - Click **Next**.
   - Click **Create Alarm**.

## Conclusion

Now, as soon as your AWS account charges exceed the set threshold (e.g., $5), you will receive a billing alert.

Feel free to use this documentation as a guide to create your billing alarm in AWS CloudWatch. If you have any questions or need further assistance, reach out for help!
