# Step to deploy the Fortinet firewall in Docker

## Sign in the Fortinet support portal
You can download the FortiGate VM QCOW2 image from the official Fortinet Support Portal. Here’s how:

### Step 1: Register for a Fortinet Account
```
Go to Fortinet Support Portal
Click "Create an Account" (if you don’t have one).
Complete the registration and verify your email.
Step 2: Download the FortiGate VM Image
Login to Fortinet Support.
Navigate to:
Download > VM Images
Select FortiGate and choose the version you need.
In the platform list, select KVM (which provides a .qcow2 image).
Click Download.
Step 3: Extract the QCOW2 Image
Once downloaded, extract the .zip file to get the fortios.qcow2 file.
```
### Step 2: install ubuntu in laptop or Cloud

### Step3: Docker installation
```bash
sudo apt-get update
sudo apt-get upgrade -y
sudo apt-get install docker.io
```
### Step 4: Clone the repo
```
git clone <repo url>
```
### Step 5: 
