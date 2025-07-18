# 🚀 AWS Networking Project: Create Your First VPC

Welcome to your very first **AWS Networking Project**! In this project, you'll learn how to build a **Virtual Private Cloud (VPC)** from scratch — the foundation of cloud infrastructure on AWS.

---

## 📘 What You'll Learn

- What a **VPC** is and why it's important.
- How to create a **public subnet** inside a VPC.
- How to attach an **Internet Gateway** to enable internet access.
- Basic networking concepts in the AWS Cloud.

---

## 🧠 Concept Overview

Imagine your AWS Region is like a **country**, and your **VPC** is your **private city** within that country.

- 🏙️ **VPC**: A private network environment inside AWS.
- 🏘️ **Subnet**: A neighborhood inside your VPC.
- 🚪 **Internet Gateway**: A door that allows your VPC to access the internet.
- 🛡️ **Route Table**: Controls how traffic flows between your resources.

---

## 🔨 Steps to Complete This Project

### 1️⃣ Create a VPC

- Go to the **VPC Dashboard** in AWS.
- Click **Create VPC**.
- Select **VPC Only**.
- Enter the following:
  - **Name**: `MyFirstVPC`
  - **IPv4 CIDR Block**: `10.0.0.0/16`
- Click **Create VPC**.

### 2️⃣ Create a Public Subnet

- Go to **Subnets** → **Create Subnet**.
- Choose the VPC you created above.
- Enter:
  - **Name**: `PublicSubnet`
  - **Availability Zone**: Choose any (e.g., `us-east-1a`)
  - **CIDR block**: `10.0.1.0/24`
- Click **Create Subnet**.

### 3️⃣ Create and Attach an Internet Gateway

- Go to **Internet Gateways** → **Create Internet Gateway**.
- Name it: `MyIGW`
- Click **Create** and then **Attach to VPC**.
- Select your `MyFirstVPC`.

### 4️⃣ Update Route Table for Internet Access

- Go to **Route Tables**.
- Find the one associated with your VPC.
- Click **Edit Routes** → **Add Route**:
  - Destination: `0.0.0.0/0`
  - Target: Your **Internet Gateway**
- Click **Save routes**.

- Then click **Subnet Associations** → **Edit subnet associations** → select `PublicSubnet`.

---

## 🎬 Demo Video

Check out our full walkthrough with **Natasha**:  
🎥 [Click here to watch the video demo](#)

---

## ✅ Outcome

By the end of this project, you’ll have:

- A fully functional **VPC**
- A **public subnet** that can reach the internet
- A solid foundation to build more advanced AWS architectures

---

## 🧰 Requirements

- AWS account
- Basic understanding of AWS Console navigation

---

## 🏁 Next Steps

- Launch an EC2 instance in the public subnet
- Associate a security group
- SSH into the instance to test internet access

---

Happy Cloud Building! ☁️✨
