# How to partition, format, and mount your block storage

Here are the steps to quick format and permanently mount an additional hard drive in Linux (Debian/Ubuntu):

1. Open a ticket and make sure we have mounted your additional large storage. Once we have done so, you will be notified and your VPS will need to be restarted for the disk to be visible to the OS.

2. SSH to your server and use the command <code>lsblk</code> to check the name and partition of the newly added hard drive. It will be listed as a block device and will typically be named <code>/dev/sdb</code>

3. Use the command <code>fdisk /dev/sdb</code> (or the appropriate name for your hard drive in place of 'sdb') to open the fdisk utility and partition the hard drive.

4. Use the command <code>n</code> to create a new partition, then <code>p</code> to create a primary partition. Select the default options for the first and last sectors to create a partition that fills the entire hard drive.

5. Use the command <code>w</code> to write the changes to the hard drive and exit fdisk.

6. Format the new partition using the command <code>mkfs.ext4 /dev/sdb1</code> (or the appropriate name for your partition). This process will take a few minutes depending on the size of your block storage, be patient.

7. Create a mount point for the new partition using the command <code>mkdir /hdd</code>.

8. Use the command <code>mount /dev/sdb1 /hdd</code> to mount the new partition.

9. To make the partition mount automatically on boot, add the following line to the file /etc/fstab: <code>/dev/sdb1 /hdd ext4 defaults 0 0</code>

10. Verify the new partition is properly mounted by using the command <code>df -h</code>. This should show /dev/sdb1 and it's size mounted to /hdd

11. That's it! Enjoy your new persistent large storage space.

Notes: The above instructions are very simplistic and generated with Debian/Ubuntu in mind, use ext4 file system, and make some basic assumptions about disk name and where to mount.