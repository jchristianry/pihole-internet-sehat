Pihole-Internetsehat
=
ULO ISP pada DNS Pi-Hole By Julius
=
**Perintah Update Pi-Hole**
```
#pihole -up
```
**Jangan lupa di-update ya, dengan perintah**
```
#pihole -g
```

**Jangan lupa configurasi mode Blocking nanti di Hasil Hostname pada cmd nslookup " domain kamu"**

**Cari di FTP : /etc/pihole/pihole-FTL.conf atau boleh perintah  nano /etc/pihole/pihole-FTL.conf**


**tambah baris bawah dan langsung copy ke nano pihole-FTL**
```
PRIVACYLEVEL=0
Blocking=IP-NODATA-AAAA
RATE_LIMIT=1000/60
PIHOLE_PTR=HOSTNAME
MAXDBDAYS=0
DBIMPORT=no
```

**Jika sudah terus save dan perintah**
```
#pihole restartdns
