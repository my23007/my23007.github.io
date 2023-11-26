---
layout: post
title: Module 2 scanning activity
subtitle: Summary
categories: scanning activity
tags: [Cyber security, Essex, Network security]
---

## Module 2 scanning activity output

Website: https://buymenow.org.uk/

C:\Users\myounes>tracert buymenow.org.uk

Tracing route to buymenow.org.uk [68.66.247.187]
over a maximum of 30 hops:

  1    <1 ms    <1 ms    <1 ms  192.168.1.1
  2     2 ms     1 ms     1 ms  100.100.64.1
  3     4 ms     3 ms     3 ms  172.21.2.177
  4     5 ms     6 ms     9 ms  10.222.225.193
  5    13 ms     4 ms     9 ms  10.222.225.186
  6    12 ms    10 ms     9 ms  172.21.0.2
  7    11 ms     5 ms     5 ms  172.21.170.12
  8     8 ms    13 ms     7 ms  172.16.70.65
  9     *        *        *     Request timed out.
 10     6 ms     7 ms    11 ms  172.16.49.1
 11     *       45 ms    45 ms  213.242.116.233
 12     *        *        *     Request timed out.
 13    59 ms   126 ms    65 ms  be2779.ccr41.par01.atlas.cogentco.com [154.54.72.109]
 14    65 ms    66 ms    70 ms  be12265.ccr41.ams03.atlas.cogentco.com [130.117.2.141]
 15    78 ms    64 ms    64 ms  be2278.rcr21.b038092-0.ams03.atlas.cogentco.com [130.117.50.250]
 16    70 ms    74 ms    64 ms  euroaccess-ltd.demarc.cogentco.com [149.6.128.82]
 17    65 ms    71 ms    67 ms  190.92.144.11.static.a2webhosting.com [190.92.144.11]
 18    64 ms    64 ms    69 ms  68.66.247.187.static.a2webhosting.com [68.66.247.187]

Trace complete.

C:\Users\myounes>

C:\Users\myounes>nslookup buymenow.org.uk
Server:  n-cns-1.terra.net.lb
Address:  213.204.78.77

Non-authoritative answer:
Name:    buymenow.org.uk
Address:  68.66.247.187


C:\Users\myounes>

 dig buymenow.org.uk     

; <<>> DiG 9.18.16-1-Debian <<>> buymenow.org.uk
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 38756
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 4096
; COOKIE: 896640820cc98ef049d179b0655b296f261d30f68b1667a8 (good)
;; QUESTION SECTION:
;buymenow.org.uk.               IN      A

;; ANSWER SECTION:
buymenow.org.uk.        13321   IN      A       68.66.247.187

;; Query time: 12 msec
;; SERVER: 213.204.78.77#53(213.204.78.77) (UDP)
;; WHEN: Mon Nov 20 04:39:58 EST 2023
;; MSG SIZE  rcvd: 88

                                                                             
┌──(kali㉿kali)-[~]
└─$ 



dig buymenow.org.uk A

; <<>> DiG 9.18.16-1-Debian <<>> buymenow.org.uk A
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 7284
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 4096
; COOKIE: 57f16de3314fc99186138dc6655b29ea0e359dfbffeed84a (good)
;; QUESTION SECTION:
;buymenow.org.uk.               IN      A

;; ANSWER SECTION:
buymenow.org.uk.        13198   IN      A       68.66.247.187

;; Query time: 4 msec
;; SERVER: 213.204.78.77#53(213.204.78.77) (UDP)
;; WHEN: Mon Nov 20 04:42:01 EST 2023
;; MSG SIZE  rcvd: 88

                                                                             
┌──(kali㉿kali)-[~]
└─$ dig buymenow.org.uk MX

; <<>> DiG 9.18.16-1-Debian <<>> buymenow.org.uk MX
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 15958
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 4096
; COOKIE: ad8124b0c2442e5663e203b3655b29fdd15c6d9e4cd838b8 (good)
;; QUESTION SECTION:
;buymenow.org.uk.               IN      MX

;; ANSWER SECTION:
buymenow.org.uk.        14400   IN      MX      0 mail.buymenow.org.uk.

;; Query time: 76 msec
;; SERVER: 213.204.78.77#53(213.204.78.77) (UDP)
;; WHEN: Mon Nov 20 04:42:20 EST 2023
;; MSG SIZE  rcvd: 93

                                                                             
┌──(kali㉿kali)-[~]
└─$ dig buymenow.org.uk NS

; <<>> DiG 9.18.16-1-Debian <<>> buymenow.org.uk NS
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 25244
;; flags: qr rd ra; QUERY: 1, ANSWER: 4, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 4096
; COOKIE: e94cfc3bbfb97ba514fbcd88655b2a0b783ece2896998624 (good)
;; QUESTION SECTION:
;buymenow.org.uk.               IN      NS

;; ANSWER SECTION:
buymenow.org.uk.        20167   IN      NS      ns2.a2hosting.com.
buymenow.org.uk.        20167   IN      NS      ns4.a2hosting.com.
buymenow.org.uk.        20167   IN      NS      ns1.a2hosting.com.
buymenow.org.uk.        20167   IN      NS      ns3.a2hosting.com.

;; Query time: 68 msec
;; SERVER: 213.204.78.77#53(213.204.78.77) (UDP)
;; WHEN: Mon Nov 20 04:42:34 EST 2023
;; MSG SIZE  rcvd: 157

                                                                             
┌──(kali㉿kali)-[~]
└─$ dig buymenow.org.uk SOA

; <<>> DiG 9.18.16-1-Debian <<>> buymenow.org.uk SOA
;; global options: +cmd
;; Got answer:
;; ->>HEADER<<- opcode: QUERY, status: NOERROR, id: 41590
;; flags: qr rd ra; QUERY: 1, ANSWER: 1, AUTHORITY: 0, ADDITIONAL: 1

;; OPT PSEUDOSECTION:
; EDNS: version: 0, flags:; udp: 4096
; COOKIE: 9fbe581e88dcde51ebb2cb6e655b2a1d6180fceca6e9e121 (good)
;; QUESTION SECTION:
;buymenow.org.uk.               IN      SOA

;; ANSWER SECTION:
buymenow.org.uk.        86400   IN      SOA     ns1.a2hosting.com. root.nl1-ss5.a2hosting.com. 2022042704 3600 1800 1209600 86400

;; Query time: 76 msec
;; SERVER: 213.204.78.77#53(213.204.78.77) (UDP)
;; WHEN: Mon Nov 20 04:42:52 EST 2023
;; MSG SIZE  rcvd: 138

                                                                             
┌──(kali㉿kali)-[~]
└─$ 


How many hops from your machine to your assigned website? 18
Which step causes the biggest delay in the route? What is the average duration of that delay? around 100 ms
What are the main nameservers for the website? ns1.a2hosting.com to ns4.a2hosting.com
Who is the registered contact? whois command
What is the MX record for the website? buymenow.org.uk.        14400   IN      MX      0 mail.buymenow.org.uk.
Where is the website hosted? 68.66.247.187.static.a2webhosting.com

## Module 2 scanning activity using nmap

command syntax: nmap -sV -T4 -O -A buymenow.org.uk

Starting Nmap 7.94 ( https://nmap.org ) at 2023-11-26 11:35 Middle East Standard Time
Nmap scan report for buymenow.org.uk (68.66.247.187)
Host is up (0.032s latency).
rDNS record for 68.66.247.187: 68.66.247.187.static.a2webhosting.com
Not shown: 905 filtered tcp ports (no-response), 9 filtered tcp ports (port-unreach), 73 closed tcp ports (reset)
PORT     STATE SERVICE    VERSION
21/tcp   open  ftp        Pure-FTPd
|_ssl-date: TLS randomness does not represent time
| ssl-cert: Subject: commonName=nl1-ss5.a2hosting.com
| Subject Alternative Name: DNS:nl1-ss5.a2hosting.com, DNS:mail.nl1-ss5.a2hosting.com, DNS:www.nl1-ss5.a2hosting.com
| Not valid before: 2023-10-20T00:00:00
|_Not valid after:  2024-01-18T23:59:59
53/tcp   open  domain     ISC BIND 9.11.4-P2 (RedHat Enterprise Linux 7)
| dns-nsid: 
|_  bind.version: 9.11.4-P2-RedHat-9.11.4-26.P2.el7_9.15
80/tcp   open  http       Apache httpd (W3 Total Cache/0.9.4.6.4)
|_http-server-header: Apache
|_http-title: 403 Forbidden
110/tcp  open  pop3       Dovecot pop3d
| ssl-cert: Subject: commonName=nl1-ss5.a2hosting.com
| Subject Alternative Name: DNS:nl1-ss5.a2hosting.com, DNS:mail.nl1-ss5.a2hosting.com, DNS:www.nl1-ss5.a2hosting.com
| Not valid before: 2023-10-20T00:00:00
|_Not valid after:  2024-01-18T23:59:59
|_ssl-date: TLS randomness does not represent time
|_pop3-capabilities: PIPELINING AUTH-RESP-CODE STLS TOP UIDL RESP-CODES SASL(PLAIN LOGIN) CAPA USER
143/tcp  open  imap       Dovecot imapd
| ssl-cert: Subject: commonName=nl1-ss5.a2hosting.com
| Subject Alternative Name: DNS:nl1-ss5.a2hosting.com, DNS:mail.nl1-ss5.a2hosting.com, DNS:www.nl1-ss5.a2hosting.com
| Not valid before: 2023-10-20T00:00:00
|_Not valid after:  2024-01-18T23:59:59
|_ssl-date: TLS randomness does not represent time
|_imap-capabilities: ID LITERAL+ SASL-IR AUTH=LOGINA0001 IMAP4rev1 capabilities more OK AUTH=PLAIN LOGIN-REFERRALS NAMESPACE have IDLE post-login STARTTLS listed ENABLE Pre-login
443/tcp  open  ssl/http   Apache httpd (W3 Total Cache/0.9.4.6.4)
|_http-server-header: Apache
|_http-title: 403 Forbidden
|_ssl-date: TLS randomness does not represent time
| ssl-cert: Subject: commonName=buymenow.org.uk
| Subject Alternative Name: DNS:buymenow.org.uk, DNS:autodiscover.buymenow.org.uk, DNS:buymenow.tech-sourcery.co.uk, DNS:cpanel.buymenow.org.uk, DNS:cpcalendars.buymenow.org.uk, DNS:cpcontacts.buymenow.org.uk, DNS:mail.buymenow.org.uk, DNS:webdisk.buymenow.org.uk, DNS:webmail.buymenow.org.uk, DNS:www.buymenow.org.uk, DNS:www.buymenow.tech-sourcery.co.uk
| Not valid before: 2023-10-11T00:00:00
|_Not valid after:  2024-01-09T23:59:59
465/tcp  open  ssl/smtp   Exim smtpd 4.96.2
|_ssl-date: TLS randomness does not represent time
| ssl-cert: Subject: commonName=buymenow.org.uk
| Subject Alternative Name: DNS:buymenow.org.uk, DNS:autodiscover.buymenow.org.uk, DNS:buymenow.tech-sourcery.co.uk, DNS:cpanel.buymenow.org.uk, DNS:cpcalendars.buymenow.org.uk, DNS:cpcontacts.buymenow.org.uk, DNS:mail.buymenow.org.uk, DNS:webdisk.buymenow.org.uk, DNS:webmail.buymenow.org.uk, DNS:www.buymenow.org.uk, DNS:www.buymenow.tech-sourcery.co.uk
| Not valid before: 2023-10-11T00:00:00
|_Not valid after:  2024-01-09T23:59:59
| smtp-commands: nl1-ss5.a2hosting.com Hello buymenow.org.uk [213.204.87.103], SIZE 78643200, 8BITMIME, PIPELINING, PIPECONNECT, AUTH PLAIN LOGIN, HELP
|_ Commands supported: AUTH HELO EHLO MAIL RCPT DATA BDAT NOOP QUIT RSET HELP
587/tcp  open  smtp       Exim smtpd 4.96.2
| ssl-cert: Subject: commonName=buymenow.org.uk
| Subject Alternative Name: DNS:buymenow.org.uk, DNS:autodiscover.buymenow.org.uk, DNS:buymenow.tech-sourcery.co.uk, DNS:cpanel.buymenow.org.uk, DNS:cpcalendars.buymenow.org.uk, DNS:cpcontacts.buymenow.org.uk, DNS:mail.buymenow.org.uk, DNS:webdisk.buymenow.org.uk, DNS:webmail.buymenow.org.uk, DNS:www.buymenow.org.uk, DNS:www.buymenow.tech-sourcery.co.uk
| Not valid before: 2023-10-11T00:00:00
|_Not valid after:  2024-01-09T23:59:59
|_ssl-date: TLS randomness does not represent time
| smtp-commands: nl1-ss5.a2hosting.com Hello buymenow.org.uk [213.204.87.103], SIZE 78643200, 8BITMIME, PIPELINING, PIPECONNECT, AUTH PLAIN LOGIN, STARTTLS, HELP
|_ Commands supported: AUTH STARTTLS HELO EHLO MAIL RCPT DATA BDAT NOOP QUIT RSET HELP
993/tcp  open  ssl/imap   Dovecot imapd
|_ssl-date: TLS randomness does not represent time
|_imap-capabilities: ID LITERAL+ SASL-IR AUTH=LOGINA0001 have capabilities OK AUTH=PLAIN LOGIN-REFERRALS NAMESPACE more IMAP4rev1 post-login ENABLE listed IDLE Pre-login
| ssl-cert: Subject: commonName=nl1-ss5.a2hosting.com
| Subject Alternative Name: DNS:nl1-ss5.a2hosting.com, DNS:mail.nl1-ss5.a2hosting.com, DNS:www.nl1-ss5.a2hosting.com
| Not valid before: 2023-10-20T00:00:00
|_Not valid after:  2024-01-18T23:59:59
995/tcp  open  ssl/pop3   Dovecot pop3d
|_ssl-date: TLS randomness does not represent time
|_pop3-capabilities: PIPELINING AUTH-RESP-CODE UIDL RESP-CODES SASL(PLAIN LOGIN) USER CAPA TOP
| ssl-cert: Subject: commonName=nl1-ss5.a2hosting.com
| Subject Alternative Name: DNS:nl1-ss5.a2hosting.com, DNS:mail.nl1-ss5.a2hosting.com, DNS:www.nl1-ss5.a2hosting.com
| Not valid before: 2023-10-20T00:00:00
|_Not valid after:  2024-01-18T23:59:59
2525/tcp open  smtp       Exim smtpd 4.96.2
|_ssl-date: TLS randomness does not represent time
| ssl-cert: Subject: commonName=buymenow.org.uk
| Subject Alternative Name: DNS:buymenow.org.uk, DNS:autodiscover.buymenow.org.uk, DNS:buymenow.tech-sourcery.co.uk, DNS:cpanel.buymenow.org.uk, DNS:cpcalendars.buymenow.org.uk, DNS:cpcontacts.buymenow.org.uk, DNS:mail.buymenow.org.uk, DNS:webdisk.buymenow.org.uk, DNS:webmail.buymenow.org.uk, DNS:www.buymenow.org.uk, DNS:www.buymenow.tech-sourcery.co.uk
| Not valid before: 2023-10-11T00:00:00
|_Not valid after:  2024-01-09T23:59:59
| smtp-commands: nl1-ss5.a2hosting.com Hello buymenow.org.uk [213.204.87.103], SIZE 78643200, 8BITMIME, PIPELINING, PIPECONNECT, AUTH PLAIN LOGIN, STARTTLS, HELP
|_ Commands supported: AUTH STARTTLS HELO EHLO MAIL RCPT DATA BDAT NOOP QUIT RSET HELP
3306/tcp open  mysql      MySQL 5.5.5-10.5.22-MariaDB-cll-lve
| mysql-info: 
|   Protocol: 10
|   Version: 5.5.5-10.5.22-MariaDB-cll-lve
|   Thread ID: 2720545
|   Capabilities flags: 63486
|   Some Capabilities: Support41Auth, Speaks41ProtocolOld, ConnectWithDatabase, SupportsTransactions, SupportsLoadDataLocal, LongColumnFlag, FoundRows, IgnoreSigpipes, InteractiveClient, SupportsCompression, ODBCClient, DontAllowDatabaseTableColumn, IgnoreSpaceBeforeParenthesis, Speaks41ProtocolNew, SupportsAuthPlugins, SupportsMultipleStatments, SupportsMultipleResults
|   Status: Autocommit
|   Salt: IiVQsq^aOEM3U5GFjb/^
|_  Auth Plugin Name: mysql_native_password
5432/tcp open  postgresql PostgreSQL DB 9.6.20 - 9.6.23 or 11.14 - 11.17
Device type: general purpose|firewall
Running (JUST GUESSING): Linux 3.X|4.X|2.6.X (85%), SonicWALL embedded (85%)
OS CPE: cpe:/o:linux:linux_kernel:3 cpe:/o:linux:linux_kernel:4 cpe:/o:linux:linux_kernel:2.6.32 cpe:/o:sonicwall:aventail_ex-1500
Aggressive OS guesses: Linux 3.10 - 4.11 (85%), Linux 3.8 (85%), Linux 4.4 (85%), Linux 2.6.32 (85%), SonicWALL Aventail EX-1500 SSL VPN appliance (85%)
No exact OS matches for host (test conditions non-ideal).
Network Distance: 7 hops
Service Info: Host: nl1-ss5.a2hosting.com; OS: Linux; CPE: cpe:/o:redhat:enterprise_linux:7

TRACEROUTE (using port 80/tcp)
HOP RTT      ADDRESS
1   1.00 ms  www.netis.cc (192.168.1.1)
2   1.00 ms  100.100.64.1
3   4.00 ms  172.21.2.177
4   6.00 ms  10.222.225.193
5   5.00 ms  10.222.225.186
6   43.00 ms 172.21.0.2
7   12.00 ms 68.66.247.187.static.a2webhosting.com (68.66.247.187)

OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 45.65 seconds
