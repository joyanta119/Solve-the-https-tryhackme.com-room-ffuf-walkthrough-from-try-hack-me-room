**Task 2:**
Command:	ffuf	-u	http://10.48.151.88/FUZZ	-w
/usr/share/wordlists/SecLists/Discovery/Web-Content/big.txt

**Task 3:**
Command	1:ffuf	-u	http://10.48.151.88/FUZZ	-w
/usr/share/wordlists/SecLists/Discovery/Web-Content/raft-medium-files-lowercas e.txt
 
Command	2:ffuf	-u	http://10.48,151.88/indexFUZZ	-w
/usr/share/wordlists/SecLists/Discovery/Web-Content/web-extensions.txt
Command	3:ffuf	-u	http://10.48.151.88/FUZZ	-w
/usr/share/wordlists/secLists/Discovery/Web-Content/raft-medium-words-lowerc ase.txt -e .php,.txt
Command	4:ffuf	-u	http://10.48.151.88/FUZZ	-w
/usr/share/wordlists/SecLists/Discovery/Web-Content/raft-medium-directories-lo wercase.txt


**Task -4**
command	1:	ffuf	-u	http://10.48.175.119/FUZZ	-w
/usr/share/wordlists/SecLists/Discovery/Web-Content/raft-medium-files-lowercas e.txt -fc 403
command	2:	ffuf	-u	http://10.48.175.119/FUZZ	-w
/usr/share/wordlists/SecLists/Discovery/Web-Content/raft-medium-files-lowercas e.txt -mc 200
command	3:	ffuf	-u	http://10.48.175.119/FUZZ	-w
/usr/share/wordlists/SecLists/Discovery/Web-Content/raft-medium-files-lowercas e.txt -fr '/\..*'


**Task 5:**
command 1: $ ffuf -u 'http://10.48.175.119/sqli-labs/Less-1/?FUZZ=1' -c -w
/usr/share/wordlists/SecLists/Discovery/Web-Content/burp-parameter-names.txt
-fw 39
command 2: :~/ffuf# for i in {0..255}; do echo $i; done | ffuf -u 'http://10.48.175.119/sqli-labs/Less-1/?id=FUZZ' -c -w - -fw 33
command  3:  :~/ffuf#  ffuf  -u  http://10.48.175.119/sqli-labs/Less-11/  -c  -w
/usr/share/wordlists/SecLists/Passwords/Leaked-Databases/hak5.txt -X POST -d 'uname=Dummy&passwd=FUZZ&submit=Submit' -fs 1435 -H 'Content-Type: application/x-www-form-urlencoded'


**Task 6:**
ffuf	-u	http://FUZZ.mydomain.com	-c	-w
/usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt -fs 0
ffuf	-u	http://mydomain.com	-c	-w
/usr/share/wordlists/SecLists/Discovery/DNS/subdomains-top1million-5000.txt -H 'Host: FUZZ.mydomain.com' -fs 0


**Task 7:**
ffuf	-u	http://MACHINE_IP/FUZZ	-c	-w
/usr/share/wordlists/SecLists/Discovery/Web-Content/common.txt	-x http://127.0.0.1:8080


ffuf	-u	http://MACHINE_IP/FUZZ	-c	-w
/usr/share/wordlists/SecLists/Discovery/Web-Content/common.txt -replay-proxy http://127.0.0.1:8080


