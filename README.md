# CLOUD-STORAGE-CREATION-S3-AND-LAUNCHING-AN-EC2-INSTANCE-IN-AWS-

### NAME: JAGAN KUMAR V

### REG NO: 212225100018

### DATE: 31-10-2026

# Experiment No. 2

# CLOUD STORAGE CREATION (S3) AND LAUNCHING AN EC2 INSTANCE IN AWS

## Aim

To create an Amazon S3 (Simple Storage Service) bucket for cloud storage and launch a virtual machine using Amazon EC2 (Elastic Compute Cloud) in the AWS Management Console.

## Objectives

After completing this experiment, students will be able to:

- Understand AWS Cloud Storage (Amazon S3).
- Create and manage S3 buckets.
- Upload and organize files in cloud storage.
- Launch an EC2 virtual server.
- Connect to an EC2 instance.
- Understand cloud computing infrastructure services.

## Software Requirements

- Laptop/Desktop
- Internet Connection
- AWS Academy Learner Account / AWS Free Tier Account
- Modern Web Browser (Chrome/Edge)

## Theory

### Amazon S3 (Simple Storage Service)

Amazon S3 is an object storage service provided by AWS that stores unlimited amounts of data with high durability and availability.

### Features

- Unlimited Storage
- 99.999999999% (11 9's) Durability
- High Availability
- Secure Storage
- Versioning
- Lifecycle Management
- Encryption

---

## Part A – Creating an Amazon S3 Bucket

### Step 1

Open the AWS Console.

URL: https://aws.amazon.com/console/

### Step 2

Log in using the following method:

- Click **Sign in using root user email**.
- Enter the registered email address.
- Enter the AWS password.
- Complete the verification process.



### Step 3

Type **S3** in the search box.

### Step 4

Click **Amazon S3**.

### Step 5

Click **Create bucket**.

### Step 6

Enter the following details:

| Parameter | Value |
|---|---|
| Bucket type | General purpose |
| Bucket name | student-cloud-storage-001 |
| AWS Region | Asia Pacific (Mumbai) |

### Step 7

Leave the remaining settings unchanged.

### Step 8

Click **Create bucket**.

### Step 9

Click **Upload**.

### Step 10

Upload the following files:

- PDF file
- Word document
- Image file

**Example:**

```text
student-cloud-storage-001
│
├── Cloud.pdf
├── Assignment.docx
├── Image.jpg
└── Notes.pdf
```


### OUTPUT

<img width="1917" height="922" alt="image" src="https://github.com/user-attachments/assets/5a800b09-199e-44c5-8a59-9454eb225c69" />


---

## Part B – Launching an Amazon EC2 Instance

### Step 1

Type **EC2** in the AWS search bar.

### Step 2

Open the **EC2 Dashboard**.

### Step 3

Click **Launch instance**.

### Step 4

Enter the instance name:

`CloudLabVM`

### Step 5

Select the operating system:

- Amazon Linux 2023
- Ubuntu Server

### Step 6

Select the instance type:

`t3.micro`

### Step 7

Create a key pair.

| Parameter | Value |
|---|---|
| Key pair name | CloudLabKey |
| Key pair type | RSA |
| File format | .pem |

### Step 8

Download the `CloudLabKey.pem` file.

### Step 9

Configure the network settings:

- Allow SSH traffic (Port 22)
- Allow HTTP traffic (Port 80)
- Allow HTTPS traffic (Port 443)

### Step 10

Set the storage size:

`8 GiB`

### Step 11

Click **Launch instance**.

### Step 12

Wait until the status changes:

```text
Pending
   ↓
Running
```



### OUTPUT

<img width="1917" height="1017" alt="Screenshot 2026-10-31 102646" src="https://github.com/user-attachments/assets/e0763235-9753-45a6-a97a-b2c5234e48cb" />


---

## Connecting to the EC2 Instance

### Step 1

Open EC2.

### Step 2

Select the instance.

### Step 3

Click **Connect**.

### Step 4

Select **EC2 Instance Connect**.

### Step 5

Click **Connect**.

### Step 6

Execute the following command:

```bash
echo "Hello AWS"
```

**Output:**

```text
Hello AWS
```


### OUTPUT

<img width="1917" height="1023" alt="Screenshot 2026-10-31 105050" src="https://github.com/user-attachments/assets/f4ad0e1c-a93b-4b34-85c0-74fc2bd349fa" />


---

## Stopping the EC2 Instance

### Step 1

Open EC2.

### Step 2

Select **Instances**.

### Step 3

Select the running instance.

### Step 4

Click **Instance state**.

### Step 5

Click **Stop instance**.

**Status:**

```text
Running
   ↓
Stopping
   ↓
Stopped
```

### OUTPUT

<img width="1917" height="967" alt="Screenshot 2026-10-31 105624" src="https://github.com/user-attachments/assets/4762d273-cabf-419c-a59b-2a4293f9061a" />


---

## Logging Out of AWS

1. Click the profile icon in the upper-right corner.
2. Select **Sign out**.

---

## Result

The Amazon S3 bucket was created successfully, files were uploaded, an EC2 instance was launched, and the virtual machine was connected successfully.
