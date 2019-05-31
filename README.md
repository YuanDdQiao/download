# download
# [禁止写磁盘]

#在根分区

mount -o ro,remount /

#非在根分区   假设文件在分区 /dev/sda3 中，该分区挂载到 /data

umount /dev/sda3 

或者命令：

umount /data 


#当然也可以设置为只读

mount -o remount,ro /data

#注意：一般推荐进入单用户模式来恢复文件
