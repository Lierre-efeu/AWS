# All About Connecting to an Instance (Work In Progress pa po)
An **EC2 instance** is a virtual server in Amazon's Elastic Compute Cloud (EC2) that provides scalable compute capacity. It allows users to run applications, host websites, or perform any kind of computation in the cloud without the need for physical hardware. The instance operates much like a physical computer, but it's managed and provisioned from the AWS platform. EC2 instances come with different configurations of CPU, memory, storage, and networking capacity, making them customizable for various workloads.

### Why do we connect to an instance?
Connecting to an instance allows an access to a server in the cloud, allowing administrators and developers to manage, configure, and maintain the infrastructure remotely. By connecting, we can install and update software, troubleshoot issues, and monitor performance. It ensures that cloud-hosted services are secure and functions efficiently.


## Secure Shell (SSH)
EC2 supports different methods for connecting to instances using SSH, including direct connections using an SSH client or browser-based SSH connections using EC2 Instance Connect. SSH is widely used for securely connecting to remote servers, particularly Linux-based systems. Additionally, every connection attempt via SSH is logged, making it easier to audit and track who accessed the instance. This is especially important in environments with multiple users and instances.


## 4 Method of Connecting to an Instance
There are 4 ways of connecting to an instance. Amazon EC2 offers various methods for connecting to instances depending on the operating system of the instance and the user's needs. Each of these ways has distinct use cases, security mechanisms, and platform compatibility.
1. **EC2 Instance Connect**
2. **SSH Client**
3. **Remote Desktop Protocol (RDP)**
4. **Session Manager**

In this workshop, let us discuss the first three ways to connect to an instance.

## Method 1: EC2 Instance Connect
Connecting via **EC2 Instance Connect** is a feature that enables a secure connection to your Linux instances over SSH. EC2 Instance Connect allows you to connect to your instance directly through your browser. It refers to the feature in Amazon Web Services (AWS) that enables users to connect to their EC2 instances using SSH through the AWS Management Console, without the need for a standalone SSH client. It allows you to use AWS Identity and Access Management (IAM) policies and users to control SSH access without needing to share or manage SSH keys. 

**Prerequisites for installing and using EC2 Instance Connect:**

*1. Install EC2 Instance Connect
2. Ensure network connectivity
3. Allow inbound SSH traffic
4. Grant permissions
5. Install an SSH client on your local computer
6. Meet username requirements*
    
## Method 2: SSH Client
Connecting to an instance through **SSH Client** involves using encryption and key-pair authentication when connectung to EC2 Linux instances. This method enables us ti associate with **key pair**.

*INTRODUCTION OF KEYPAIR*

**Public Key** - stored on the EC2 instance and can be shared publicly

**Private Key** - stored seccurely on the local machine, ensuring that only authorize users can connect to the EC2 environment


## Method 3: Remote Desktop Protocol (RDP)
**Remote Desktop Protocol (RDP)** enables multiple users to connect to a window instances. Users can have separate sessions on the same server, allowing them to run different applications, access different files, and have their own desktop environments without interfering with each other’s work.

**Prerequisite for Connecting Instance using RDP**

**Install an RDP client** - allows to connect to and interact with a remote Windows instance

