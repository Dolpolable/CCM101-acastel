
# Laboratory Activity 2 – Build the Cloud Infrastructure Blueprint

## About the Activity

This laboratory activity focused on learning the basic parts of cloud infrastructure. I used the KillerCoda Playground to work with an Ubuntu Linux server and collect information about its system resources.

During the activity, I investigated the server's operating system, CPU, memory, storage, and network information. I also researched cloud providers, created a simple cloud infrastructure diagram, and organized the laboratory files using Git and GitHub.

## What I Did

The main tasks completed in this laboratory were:

* Checked the Ubuntu operating system and kernel.
* Identified the CPU and available processing resources.
* Checked the server's memory.
* Examined the available storage and disk space.
* Checked the hostname and IP address.
* Researched AWS, Microsoft Azure, and Google Cloud.
* Compared common cloud services.
* Created a simple cloud infrastructure diagram.
* Created and organized the laboratory files.
* Uploaded the completed work to GitHub.

## System Information

The Linux server used in the activity had the following basic information:

* **Operating System:** Ubuntu 24.04.4 LTS
* **Codename:** Noble
* **Kernel:** 6.8.0-138-generic
* **CPU:** Intel Xeon E312xx (Sandy Bridge, IBRS update)
* **CPU Cores:** 1
* **Hostname:** ubuntu

The server information was collected using Linux terminal commands.

## Commands Used

### Checking the Operating System

```bash
lsb_release -a
uname -r
```

These commands were used to check the Ubuntu version and Linux kernel.

### Checking CPU and Memory

```bash
lscpu | grep "Model name"
nproc
free -h
```

These commands were used to identify the processor, number of CPU cores, and available memory.

### Checking Storage

```bash
df -h
```

These commands were used to check the available disk space, partitions, and storage devices.

### Checking Network Information

```bash
hostname
hostname -I
ip addr
ip route
```

These commands were used to identify the server hostname, IP addresses, network interfaces, and routing information.

## Creating the Laboratory Files

I created the main laboratory directory and files using the Ubuntu terminal.

```bash
cd ~/CCM101-cbadongen
mkdir -p Laboratory-02-Build-the-Cloud-Infrastructure-Blueprint
cd Laboratory-02-Build-the-Cloud-Infrastructure-Blueprint
mkdir screenshots
```

The Markdown files were created using:

```bash
touch README.md
touch infrastructure-report.md
touch cloud-components.md
touch cloud-provider-comparison.md
touch reflection.md
```

I used `nano` to edit the files:

```bash
nano README.md
nano infrastructure-report.md
nano cloud-components.md
nano cloud-provider-comparison.md
nano reflection.md
```

I also used `cat` to check the contents:

```bash
cat README.md
cat infrastructure-report.md
cat cloud-components.md
cat cloud-provider-comparison.md
cat reflection.md
```

## Cloud Provider Research

I researched three major cloud providers:

1. **Amazon Web Services (AWS)**
2. **Microsoft Azure**
3. **Google Cloud Platform (GCP)**

The comparison focused on their common infrastructure services, including compute, storage, networking, and identity services.

## Cloud Infrastructure Diagram

I created a simple infrastructure blueprint for a fictional company.

The diagram contained:

* **User**
* **Internet Connection**
* **Network**
* **Compute Resource**
* **Storage Resource**

The diagram was created using **draw.io** and exported as a PNG image for the laboratory output.

## GitHub

Git was used to organize and submit the laboratory activity.

The main commands used were:

```bash
git status
git add .
git commit -m "Complete Laboratory 2 cloud infrastructure blueprint"
git push
```

These commands allowed me to check the files, stage the changes, save the work in a commit, and upload the files to GitHub.

## Tools Used

* KillerCoda Playground
* Ubuntu Linux Terminal
* Git
* GitHub
* draw.io
* Google Chrome
* Markdown

## What I Learned

This activity helped me understand the basic resources found in a cloud environment. I learned how to use Linux commands to inspect a server and collect information about its CPU, memory, storage, operating system, and network.

I also learned how different cloud providers offer similar services under different names. Creating the infrastructure diagram helped me understand how users, networks, compute resources, and storage are connected.

## Challenges

One challenge was remembering which Linux command should be used for each type of system information. Another challenge was organizing the required files and screenshots correctly.

I also had to make sure that the files were properly added, committed, and pushed to GitHub.

## Laboratory Folder

The final laboratory folder contains the documentation, reports, reflection, and screenshots.

```text
Laboratory-02-Build-the-Cloud-Infrastructure-Blueprint/
├── README.md
├── infrastructure-report.md
├── cloud-components.md
├── cloud-provider-comparison.md
├── reflection.md
└── screenshots/
```

## Conclusion

Laboratory Activity 2 gave me practical experience in examining a Linux cloud environment and understanding its basic infrastructure. I learned how compute, storage, memory, networking, and the operating system work together.

The activity also improved my skills in Linux commands, cloud infrastructure, cloud provider research, Markdown, Git, GitHub, and creating a basic cloud architecture diagram.
