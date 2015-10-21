You can mount a drive partition using command line with the udisks tool. For example:

```/usr/bin/udisks --mount /dev/sdb1```

The bit after ```--mount``` is the device name of the partition you want to mount. (/dev/something). The command will mount `/dev/sdb1` in `/media/<uuid>` where `<uuid>` is the identifier of the particular partition. Read below to find the uuid of your partition. 


This will give location at which given partition is mounted. For example, if I run the command 

```/usr/bin/udisks --mount /dev/sda7```

Following will be the output:

Mounted ```/org/freedesktop/UDisks/devices/sda7``` at ```/media/New Volume```

Where ```/media/New Volume``` is the location where given drive partition ```sda7``` is mounted.

Now, this partition can be accessed using command line using the command:

```cd /media/New\ Volume/```