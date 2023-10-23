# AWS-WordPress-Website.
This repository documents the process of launching and configuring a WordPress instance using Amazon Lightsail. 

# Deploying a WordPress Instance on Amazon Lightsail

This guide provides step-by-step instructions on how to launch and configure a WordPress instance on Amazon Lightsail. By following these steps, you'll be able to set up a WordPress website quickly and efficiently.

## Prerequisites

Before you begin, ensure you have the following:

- An AWS account
- A domain name or subdomain for your website

## Step 1: Create an Amazon Lightsail Account

1. If you don't have an Amazon Lightsail account, [create one here]**(https://lightsail.aws.amazon.com/ls/webapp/account/sign-in)**.

## Step 2: Create a WordPress Instance

1. Sign in to the Lightsail console.
2. On the Instances tab, choose "Create instance."
3. Select the AWS Region and Availability Zone.
4. Choose the instance image (Linux/Unix with WordPress blueprint).
5. Select an instance plan.
6. Enter a name for your instance and choose "Create instance."

## Step 3: Connect to Your Instance via SSH

1. On the Instances tab, choose the SSH quick-connect icon for your WordPress instance.
2. Retrieve the default application password using **`cat $HOME/bitnami_application_password`**.
3. Make note of the password.

## Step 4: Sign in to the WordPress Admin Dashboard

1. In a browser, go to:** `http://PublicIpAddress/wp-login.php`** (replace PublicIpAddress with your instance's public IP address).
2. Enter the username and the default password obtained earlier.
3. Log in to your WordPress admin dashboard.

## Step 5: Create a Lightsail Static IP Address

1. On the Instances tab, choose your running WordPress instance.
2. Go to the Networking tab and create a static IP address, attaching it to your instance.

## Step 6: Create a Lightsail DNS Zone

1. On the Networking tab, create a DNS zone for your domain.
2. Add the necessary DNS records to point your domain to your WordPress instance.

## Step 7: Clean Up

1. Delete your Lightsail instance when you're done.

## Conclusion

Congratulations! You've successfully launched and deployed a WordPress instance on Amazon Lightsail. This guide can be used as a reference for future deployments.

### What's Done:
- Created a WordPress instance on Amazon Lightsail.
- Connected to the WordPress administration dashboard.
- Configured DNS settings to map the domain to the Lightsail instance.

### What's Pending:
- Customizing the WordPress website by adding content, themes, and plugins.
- Creating and publishing web pages and posts.
- Customizing the website's appearance and layout.
- Adding functionality to the website through plugins.
- Ongoing updates and content management.

For more detailed information and troubleshooting, please refer to the [official Lightsail documentation](https://lightsail.aws.amazon.com/ls/docs/en_us).


