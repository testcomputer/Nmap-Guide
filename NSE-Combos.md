  
  
  
    nmap -sV --script=vulscan/vulscan.nse www.example.com
    http-fingerprints.nikto-db-path
    http-enum.basepath
    http-enum.displayall (Careful, false positives reported)
    http-grep.nse
    http-grep.url
    ssh-brute.nse
    dns-brute.nse
    http-config-backup.nse
    vulscan.nse
    smb-enum-users.nse (Scanning for Windows Users)
    http-wordpress-enum.nse
    firewalk.nse
    mysql-empty-password.nse
    mysql-users.nse
    mysql-brute.nse

Build around --script=vulnscan/vulscan.nse
http-enum.nse
