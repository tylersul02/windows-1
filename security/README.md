<pre>

ntfs-3g /dev/sda1 /mnt/windows –o force
cd /mnt/windows/Windows/System32/config
chntpw –l SAM
chntpw –u USERNAME SAM

mount -t ntfs-3g -o remove_hiberfile /dev/sda? /mnt as an alternative.
    cd /mnt/Windows/System32/Config
    chntpw -i SAM
    Press 1
    Enter the RID of the user you wish to change the password for.
    Press 1
    Press q
    Press q
    Press y
    cd
    umount /mnt
    reboot
</pre>
