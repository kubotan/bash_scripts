*CentOS7のUSBインストールメディアを作成
+8GBくらいのUSBメモリをMacに刺す。
+Macのターミナル上で以下のコマンドを実行する
$ sh createInstallMedia.sh 


===== External Disk List =====
/dev/disk2 (external, physical):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:     FDisk_partition_scheme                        *3.9 GB     disk2
   1:                       0xEF                         6.4 MB     disk2s2


===== Download ISO List =====
/Users/hogehoge/Downloads/CentOS-7-x86_64-Minimal-1611.iso


Enter the USB storage to create the installation disk [/dev/disk2]: 
Enter the ISO file to create the installation disk [/Users/hogehoge/Downloads/CentOS-7-x86_64-Minimal-1611.iso]: 


Execute this command.

  Command:
    /usr/sbin/diskutil unMountDisk /dev/disk2
    /usr/bin/sudo /bin/dd if=/Users/hogehoge/Downloads/CentOS-7-x86_64-Minimal-1611.iso of=/dev/disk2

Do you want to continue? [Y/n]Y

Press Control + T to display the progress.
Executing...
Unmount of all volumes on disk2 was successful
1392640+0 records in
1392640+0 records out
713031680 bytes transferred in 676.196776 secs (1054474 bytes/sec)
Finished.
 