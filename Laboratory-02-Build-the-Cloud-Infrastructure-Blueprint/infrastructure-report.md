## Checkpoint 2 – Investigate the Cloud Server

This report documents the hardware, operating system, storage, and networking information collected from the Linux server using the KillerCoda Playground.

## 1. Operating System

The server is running:

**Ubuntu 24.04.4 LTS**

- Release: **24.04**
- Codename: **Noble**

## 2. Kernel Version

The Linux kernel version is:

**6.8.0-138-generic**

## 3. CPU Model

The CPU model detected on the server is:

**Intel Xeon E312xx (Sandy Bridge, IBRS update)**

The system also reports:

**RHEL-9.6.0 PC (Q35 + ICH9, 2009) CPU @ 2.0GHz**

## 4. Number of CPU Cores

The server has:

**1 CPU core**

This was determined using the `nproc` command.

## 5. Total RAM

The server has approximately:

**1.9 GiB of RAM**

The memory information reported:

| Memory | Total | Used | Free | Available |
|---|---:|---:|---:|---:|
| RAM | 1.9 GiB | 419 MiB | 853 MiB | 1.4 GiB |

The server also has:

**1.0 GiB of Swap**

## 6. Disk Capacity

The main disk has a capacity of:

**19 GB**

The `df -h` command showed:

| File System | Size | Used | Available | Mounted On |
|---|---:|---:|---:|---|
| `/dev/vda1` | 19G | 5.4G | 13G | `/` |
| `/dev/vda16` | 881M | 117M | 703M | `/boot` |
| `/dev/vda15` | 105M | 6.2M | 99M | `/boot/efi` |

## 7. Mounted File Systems

The server has several mounted file systems.

The main mounted file systems include:

- `/dev/vda1` mounted on `/`
- `/dev/vda16` mounted on `/boot`
- `/dev/vda15` mounted on `/boot/efi`
- `tmpfs` mounted on `/run`
- `tmpfs` mounted on `/dev/shm`
- `tmpfs` mounted on `/run/lock`

The main file system is `/dev/vda1`, which provides the primary storage for the Linux server.

## 8. Hostname

The hostname of the Linux server is:

**ubuntu**

This was obtained using the `hostname` command.

## 9. IP Address

The server has the following IP addresses:

**172.30.1.2**

**172.17.0.1**

These addresses were displayed using the `hostname -I` command.

## 10. Linux Commands Used

The following commands were used to investigate the cloud server:

```bash
lsb_release -a
uname -r
lscpu | grep "Model name"
nproc
free -h
df -h
hostname
hostname -I
