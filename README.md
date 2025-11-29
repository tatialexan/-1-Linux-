# -1-Linux-
Я обновила ядро, но не сохранила изменения перед перезагрузкой. Прикладываю скрин после обновления и код соотвественно. На скрине в верхней части уже обновленное ядро, ниже попыталась воспроизвести команды, которыми обновляла ядро.
Обновление ядра системы
<img width="1680" height="1050" alt="image" src="https://github.com/user-attachments/assets/2205ea46-c069-4ba6-8703-0889d1df2203" />


buntu@ubuntu:~$ uname -r 
6.14.0-27-generic
ubuntu@ubuntu:~$ mkdir kernel && cd kernel
ubuntu@ubuntu:~/kernel$ wget 
wget: missing URL
Usage: wget [OPTION]... [URL]...

Try `wget --help' for more options.
ubuntu@ubuntu:~/kernel$ sudo dpkg -i *.deb 
dpkg: error: cannot access archive '*.deb': No such file or directory
ubuntu@ubuntu:~/kernel$ ls -al /boot
total 24974
drwxr-xr-x 1 root root      202 Aug  5 17:38 .
drwxr-xr-x 1 root root      240 Nov 29 16:53 ..
-rw------- 1 root root  9145157 Aug  5 17:38 System.map-6.14.0-27-generic
-rw-r--r-- 1 root root   296154 Aug  5 17:38 config-6.14.0-27-generic
drwxr-xr-x 2 root root       58 Aug  5 17:38 grub
lrwxrwxrwx 1 root root       28 Aug  5 17:38 initrd.img -> initrd.img-6.14.0-27-generic
lrwxrwxrwx 1 root root       28 Aug  5 17:38 initrd.img.old -> initrd.img-6.14.0-27-generic
-rw-r--r-- 1 root root   142796 Apr  8  2024 memtest86+ia32.bin
-rw-r--r-- 1 root root   143872 Apr  8  2024 memtest86+ia32.efi
-rw-r--r-- 1 root root   147744 Apr  8  2024 memtest86+x64.bin
-rw-r--r-- 1 root root   148992 Apr  8  2024 memtest86+x64.efi
lrwxrwxrwx 1 root root       25 Aug  5 17:38 vmlinuz -> vmlinuz-6.14.0-27-generic
-rw------- 1 root root 15546760 Aug  5 17:38 vmlinuz-6.14.0-27-generic
lrwxrwxrwx 1 root root       25 Aug  5 17:38 vmlinuz.old -> vmlinuz-6.14.0-27-generic
ubuntu@ubuntu:~/kernel$ 
