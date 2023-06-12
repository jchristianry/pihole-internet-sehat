# pihole-internetsehat
ULO ISP  ( Trust+Positif By Kemkominfo RI ) pada DNS Pi-Hole By Julius
- Jangan lupa di-update ya, dengan perintah ' pihole -g ' atau menu Tools -> ' Update Gravity '

Jangan lupa configurasi mode Blocking nanti di Hasil Hostname pada cmd nslookup " domain kamu "
- Cari di FTP : /etc/pihole/pihole-FTL.conf atau boleh perintah  nano /etc/pihole/pihole-FTL.conf
- tambah baris bawah : 
  1. PRIVACYLEVEL=0
  2. Blocking=IP-NODATA-AAAA
  3. RATE_LIMIT=1000/60
  4. PIHOLE_PTR=HOSTNAME ( ganti hostname pi.hole menjadi HOSTNAME ).
  5. MAXDBDAYS=365 menjadi 0
  6. DBIMPORT=yes menjadi no ( agar disable database kaya reset semula database 0 )
- Jika sudah terus save dan perintah " pihole restartdns "
