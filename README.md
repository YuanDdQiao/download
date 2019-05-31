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

yum install redhat-lsb -y

# [CentOS-bin]

	~]# lsb_release -a
	LSB Version:	:...
	Distributor ID:	CentOS
	Description:	CentOS Linux release 7.4.1708 (Core) 
	Release:	7.4.1708
	Codename:	Core
https://github.com/YuanDdQiao/download/blob/master/linux/centos7.4.1708/ext3grep

~]# lsb_release -a

	LSB Version:	:...
	Distributor ID:	CentOS
	Description:	CentOS release 6.5 (Final)
	Release:	6.5
	Codename:	Final

wget https://github.com/YuanDdQiao/download/blob/master/linux/centos6.5/ext3grep