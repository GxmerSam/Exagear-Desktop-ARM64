# Fixed-image-for-Exagear-Desktop
It seems exagear stopped , by which no more updates in future, and if someone wanna install it, he can't install any app because server is off. This is my patch can by apply on newly installing exagear desktop to get updates, and fixed apt update error.
 # Warning
It is highly recommend to take backup, you will do this on your own risk. 

# Installation 


(1)To install patch, first clone it to pc:-
``` git clone https://github.com/SamarJi/Fixed-image-for-Exagear-Desktop ```

(2) Once cloned , if you got some errors while using apt update,use these commands :-
``` apt remove apt ```

That apt have bug, which cannot take updates
```dpkg -i  libapt-pkg4.12_1.0.9.8.6_i386.deb```
Then 
``` dpkg -i  apt_1.0.9.8.4_i386.deb```
(3) Replace exagear's sources.list which is located in `/opt/exagear/images/debian-9/etc/apt/sources.list` with this repositor's `sources.list`
 
(4) Once all done, you can use `apt update` can will got latest updates, don't use apt `upgrade`
