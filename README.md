# pihole-internetsehat
ULO ISP  ( Trust+Positif By Kemkominfo RI ) pada DNS Pi-Hole By Julius
Jangan lupa di-update ya, dengan perintah ' pihole -g ' atau menu Tools -> ' Update Gravity '

Jangan lupa configurasi mode Blocking nanti di Hasil Hostname pada cmd nslookup " domain kamu "
- cari di FTP : /etc/pihole/pihole-FTL.conf atau boleh perintah  nano /etc/pihole/pihole-FTL.conf
  tambah baris bawah : 
  PRIVACYLEVEL=0
  Blocking=IP-NODATA-AAAA
  RATE_LIMIT=1000/60
  PIHOLE_PTR=HOSTNAME ( ganti hostname pi.hole menjadi HOSTNAME ).
  MAXDBDAYS=365 menjadi 0
  DBIMPORT=yes menjadi no ( agar disable database kaya reset semula database 0 )
terus Save dan perintah " pihole restartdns "
