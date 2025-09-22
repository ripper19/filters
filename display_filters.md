have a standard - protocol.feature.subfeature

tcp.port==3389 Filter out RDP traffic
tcp.flags.syn==1 TCP packets with the SYN flag set
tcp.flags.reset==1 TCP packets with the RST flag set
!arp Clear ARP traffic
http All HTTP traffic
tcp.port==23 || tcp.port==21 Telnet or FTP traffic
smtp || pop || imap Email traffic (SMTP, POP, or IMAP)
