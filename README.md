# docker-armhf-snort
Dockerfile for armhf on Ubuntu14.04 in snort

# Build ths container
sudo docker build -t="{name}/{containername}:{version}" .
\n
Example
sudo docker build -t="myproject/snort:1.0" .

# Instructions

Pulledpork
sudo /usr/local/bin/pulledpork.pl -c /etc/snort/pulledpork.conf -l 
\n
Snort
sudo /usr/local/bin/snort -u snort -g snort -c /etc/snort/snort.conf -i eth0 -D
\n
Barnyard2
sudo barnyard2 -c /etc/snort/barnyard2.conf -d /var/log/snort -f snort.u2 -w /var/log/snort/barnyard2.waldo -g snort -u snort -D
