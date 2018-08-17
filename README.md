1.  Setup your own lab within vmware/virtualbox
      - Use CentOS 7 or download free copy of RHEL from redhat

2.  Create another vm. Now setup the following servers
      - Setup own LDAP server https://goo.gl/6zSgHC
      - Setup own NFS server https://goo.gl/8W6KU8
3.  Don't rely on gui. 
4.  For managing firewall, don't rely on gui also. Use #firewall-cmd command
5.  Know how to use man/info/help/locate/find/rpm -qd command
6.  Have clear understand on linux filesystem and how to work on lvm
7.  Have clear understand on filesystem extend, reduce/resize command. For example: extend the size (by using logical extent or specific     size)reduce size of partition/logical volume, resize to exact size without hampering the files on the filesystem, check the             filesystem health, labelling etc. 
8.  Have clear understand on logical extent. Here is the good topic on it https://goo.gl/wTyB3R
9.  Be familiar with RHCSA objectives.
10. Use multiple ssh window and watch audit.log, messages (tail -f) and journalctl (journalctl -xf)
11. Watch Sander van Vugt's advice on RHCSA exam https://www.youtube.com/watch?v=tok9qimRw6k
12. Every service must servive reboot. So give extra care about persistency. Reboot reboot reboot & check if everything working or not
13. Install bash-completion package (might be already installed) which help you to autocomplete any command
14. If you forgot how to setup cronjob, just look inside /etc/crontab file
15. Give extra care on:
      - File system partitioning (Use UUID when you add your file system in /etc/fstab for persistency)
      - ACL
      - firewall-cmd (with --permanent option)
      - setuid/setgid
      - File/folder permission
      - Selinux
      - Seboolean (with -P option)
      - breaking root password
      - ldap
      - autofs
      - nfs
      - network setup
      - etc

 16. Instead of memorizing big command for managing virtualization, simply remember the following group command:
     #yum groups install "Virtualization Hypervisor" "Virtualization Client" "Virtualization Tools"  "Virtualization Platform"
     Forgot that command also? No worries! just execute: #yum group list hidden
 17. If there are any filesystem related task, try to solve that task at first. Then reboot to see if your system boot properly or not.
 18. Give extra attention on time
 19. Always go through RHCSA objectives unless you feel absolutely ready
 20. Don't consult guide if you forgot anything. Just learn to use man/info/help/locate/find/rpm -qd command

# Advices
  - Use nmcli to setup your network
  - Install some useful package first. For example: yum-utils, bash-completion, setroubleshoot-server etc
  - Make sure that you know how to add new repository. Use yum-config-manager
  - In exam hall, don't be stress. Just chill. Also don't be hurry. If you complete early, just reboot the machine couples of time and check every question answers for error.
  
  
  Good luck!
  
  (last updated on 17-Aug-18)
