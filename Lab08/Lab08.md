## Lab 08

- Name: Jordan Cox
- Email: cox.389@wright.edu

## Part 1

1. Command: `lsblk`
```
xvda     202:0    0   16G  0 disk
├─xvda1  202:1    0 15.9G  0 part /
├─xvda14 202:14   0    4M  0 part
└─xvda15 202:15   0  106M  0 part /boot/efi
```
2. Command: `sudo parted /dev/xvda` `print`
```
Model: Xen Virtual Block Device (xvd)
Disk /dev/xvda: 17.2GB
Sector size (logical/physical): 512B/512B
Partition Table: gpt
Disk Flags:

Number  Start   End     Size    File system  Name  Flags
14      1049kB  5243kB  4194kB                     bios_grub
15      5243kB  116MB   111MB   fat32              boot, esp
 1      116MB   17.2GB  17.1GB  ext4
```
3. For the `xvda` partition table:
    - Does it use MBR or GPT? GPT
    - How many partitions are on the block device? 3
    - What is the largest partition? xvda1
4. Command: `blkid`
```
/dev/xvda1: LABEL="cloudimg-rootfs" UUID="b78b2f9f-3a08-427a-ad4e-4a04f235761c" BLOCK_SIZE="4096" TYPE="ext4" PARTUUID="5685b7d3-4911-4237-9405-e73d2d78ca3e"
/dev/xvda15: LABEL_FATBOOT="UEFI" LABEL="UEFI" UUID="4B1C-F903" BLOCK_SIZE="512" TYPE="vfat" PARTUUID="1dcb7fe9-f679-4d8b-afbe-2f4f444c7095"
```
5. For the primary partition:
    - What partition is the root filesystem on? xvda1
    - What is the partition label? "cloudimg-rootfs"
    - What type of filesystem is on the partition? ext4
6. Command: `df -h` 
```
Output here
```
7. For the root filesystem:
    - What is the total size?
    - How much space is used?
    - Where is it mounted to?
8. Command:
```
Output here
```
9. Fields & purpose of fields in entry that mount the root filesystem


## Part 2

1. `gdisk` main menu options
   - `p`:
   - `o`:
   - `n`:
   - `i`:
   - `w`:
2. Steps to create a partition table and partition on `xvbd`
3. Partition table on `/dev/xvdb`
```
Paste partition table information here
```
4. Answer these questions:
   
   a. What device name does the partition use?
      - Answer: 
        
   b. What size is the partition in GB?
      - Answer: 
        
   c. What filesystem type will be used on the partition?
      - Answer: 

## Part 3

1. Commands used:
2. Commands used:
```
output here
```
3. Commands used:
4. Commands used:
5. Contents of `/mnt/newworld`:
```
list here
```
6. Commands used:
7. When can I interact with files on the filesystem on the partition in `xvdb`?
   - Answer:
   
## Part 4

1. Commands used:
2. Line you added to `/etc/fstab`:
3. How did you confirm that the mount point changed? (Commands used or explain process):
4. **If you restored `/etc/fstab`**, write here why you did not feel comfortable leaving your changes in place


## Part 5

1. Commands used:
2. What does the `strings` command do?
   - Answer:
3. Write a short explanation of what you saw in `strings` output:
4. Commands used:
5. Is the secret you deleted still showing up in the `strings` output?

### Report: How to Permanently Delete a File

**Write your report here**

## Extra Credit Answers:

1. Commands used: 
2. Explanation:
3. Commands used: 
4. Commands used: 
