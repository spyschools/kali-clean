# kali-clean
Clean a Kali Linux system of unused files and directories

# sudo du -sh /var/log
2.5G /var/log

# git clone https://github.com/spyschools/kali-clean.git
# cd kali-clean

1. delete log files 
# sudo ./remove-old-logs.sh 
OR
# sudo bash remove-old-logs.sh 

Running the script in exec mode recovers significant disk space:
# sudo ./remove-old-logs.sh exec
OR
# sudo bash remove-old-logs.sh exec

2. Remove Unused Dependencies
# sudo apt autoremove -y

3. Remove Unused Kernels and Kernel Headers
# sudo ./remove-old-logs.sh 
OR
# sudo bash remove-old-kernels.sh

Running the script in exec mode recovers significant disk space:
# sudo ./remove-old-kernels.sh exec
OR
# sudo bash remove-old-kernels.sh exec

