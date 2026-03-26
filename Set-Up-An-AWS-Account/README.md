<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Set Up An AWS Account

**Project Link:** [View Project](http://learn.nextwork.org/projects/aws-account-setup)

**Author:** Emmanuel Elom Akatse  
**Email:** e.akatse@gmail.com

---

![Image](http://learn.nextwork.org/thankful_white_quiet_troll/uploads/aws-account-setup_r6s1t7u3)

---

## Introducing Today's Project!

In this project, I'm going to set up my own free-tier AWS account, learn about AWS free-tier, and configure billing alerts to avoid surprise billings.

### Key tools and concepts

The key tools I used include AWS IAM, which was useful in setting up MFA to secure my root account; Billing Preferences under Billing and Cost Management, which helped me set a usage limit target to ensure I stayed within free-tier resource utilization; and the Google Authenticator app, which assisted in setting up MFA by providing an extra layer of security for my AWS account through time-based one-time passwords (TOTP) for two-factor authentication.

Key concepts I learned include cloud cost management through AWS Free Tier usage limits, resource-based pricing models (e.g., AWS Lambda and DynamoDB quotas), and cloud security principles such as multi-factor authentication (MFA). I also gained hands-on experience implementing these concepts by configuring MFA on the root account and setting up billing alerts.


### Challenges and wins

This project took me approximately 45 minutes to complete. I didn’t face any major challenges, as everything was simple and straightforward.

---

## Creating My AWS Account

In this step, I'm going to create a new AWS account, verify my email used to create the AWS account, and create a strong root user password.

### Understanding the root user

I learned that a root user is the main owner of an AWS account and has full access to everything within it. It's sort of like having a master key to a building. Every AWS account has only one root user.
Also, it's important to have a strong password as it makes it difficult for unauthorized users to gain access to your account and use it for nefarious activities or use the account to incur unwanted charges on your account.

---

## Setting Up Billing and Payment

In this step, I'm going to set up billing by selecting a free plan, enter my contact information, and add a payment method.

### Why AWS requires a payment method

I learned that AWS requires a payment method for two reasons. First, it needs it to authenticate that you are actually a real person and not a bot trying to use free cloud resources. Second reason is, suppose your resource utilization exceeds the free-tier limits, AWS will need a way to charge you for the extra resource utilization. 

---

## Completing Account Activation

In this step, I'm going to verify my identity and select a support plan to activate my AWS account.

### Identity verification and support plan

I verified my identity by verifying phone number with my country code and received a verification code for it. 
The Basic support plan includes AWS documentation, forums, and AWS Trusted Advisor which helps you optimize your AWS resources by providing recommendations on cost optimization, performance, security, service limits, and fault tolerance.

---

## Enabling Free Tier Alerts

In this step, I'm going to enable free-tier usage alerts by navigating to `Billing Preferences` on the AWS management console.

![Image](http://learn.nextwork.org/thankful_white_quiet_troll/uploads/aws-account-setup_j6k1l7m3)

### Why usage alerts matter

I set up usage alerts because AWS will alert me if my resource utilization hits 85% on free-tier limit by sending me an email. This way, I will be able to stop or readjust my resource usage in order not incur any unwanted billing.

---

## Securing the Account with MFA

To enable MFA, I navigated to `IAM` on the AWS console. From there, I clicked on `add MFA` beside `Security recommendations` under `IAM Dashboard`.
Added my preferred device name under `MFA device name`. Selected `Authenticator app` as the MFA device type, and opened up my Google Authenticator app on my android device. I then clicked on the `Show QR code` button. Opened my authenticator app on my phone (already had it installed).
Tapped the + button (or Add account) in the app.
Selected `Scan QR code` and pointed my phone camera at the QR code on screen.

The authenticator app works by showing a 6-digit code that refreshes every 30 seconds. You enter the first code in the `MFA code 1` field. Wait for code to refresh and enter the second code in the `MFA code 2` field. Click on `Add MFA`. 
And that it. It's all set up!

![Image](http://learn.nextwork.org/thankful_white_quiet_troll/uploads/aws-account-setup_e3f7g2h8)

---

---
