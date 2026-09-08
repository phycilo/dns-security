DNS Security: Threats, Protection Methods, and Basic Analysis Introduction 

When accessing a website on the internet, we generally use domain names. When we type something into the search bar, our computer knows the IP address corresponding to that domain name. The basic system that performs this process is DNS (Domain Name System). While it's easy for people to remember domain names, computers use IP addresses for communication. However, DNS is not just a system that provides connections. When misconfigured or misused, it can lead to various security problems. Therefore, DNS security is one of the important issues of cybersecurity.

How does DNS work? 

When a user types ______.com into a browser, the computer needs to learn the IP address of that domain name.

The DNS resolver looks for the IP address of the domain by communicating with DNS servers. When it finds the correct IP address, it sends it back to the user's computer. The computer then uses this address to connect to the website. This is why DNS information needs to be correct and reliable.

Key Threats to DNS 

1. DNS Spoofing: DNS spoofing is when a user receives a fake DNS response instead of the real one. For example, if a user wants to go to: mybank.com and receives an incorrect IP address via DNS, they may be redirected to a different server. This situation can pose a risk, especially in terms of phishing and redirecting users to fake websites.

Using a VPN can reduce the risk of DNS manipulation on untrusted networks by protecting traffic between the device and the VPN server. Encrypted DNS technologies such as DoH and DoT can also improve DNS privacy. However, DNSSEC provides a different type of protection by helping verify the authenticity and integrity of DNS data.

2. DNS Cache Poisoning: DNS resolvers cache DNS responses for a certain period to improve performance. If an attacker can get a fake DNS message to be cached, the resolver can then send users the wrong IP address. Therefore, secure management of the DNS cache is important.

To protect against DNS cache poisoning attacks, it is necessary to use DNSSEC technology and choose secure DNS servers.

3. DNS Hijacking: DNS hijacking can occur by redirecting users to different addresses through unauthorized modification of DNS configuration or DNS traffic. For example, changing a device's DNS settings can send users' DNS queries to a server controlled by the attacker. 

To protect against DNS hijacking, change your modem's default administrator interface password to a strong and unique password. Turn off remote management. Disable your modem's external management feature unless absolutely necessary and use secure DNS.

4. DNS Tunneling: DNS tunneling is the misuse of the DNS protocol for transporting data outside its normal purpose. Security teams may therefore try to detect unusual queries by monitoring DNS traffic. For example, seeing a large number of meaningless and long subdomain queries may be a behavior that needs to be investigated.

To protect against DNS tunneling, continuously monitor DNS traffic on your network. Track suspicious activity such as excessively long subdomains, high data volume, or abnormal query frequency. For security, limit direct DNS requests from the internal network to the external network. Allow all DNS queries only through trusted and authorized corporate DNS servers. Use AI and signature-based security systems to detect abnormal tunneling behavior and malicious data leakage attempts early. DNSSEC can help protect the integrity and authenticity of DNS data, but it does not directly prevent DNS tunneling. DNS tunneling should be detected through DNS traffic monitoring, filtering, and analysis.

Monitoring DNS Logs

One of the important parts of DNS security is examining the logs. A security analyst can look for the following behaviors in DNS records: An unusual number of DNS queries Very long subdomains Domains consisting of random characters Suspicious or known malicious domains Queries to DNS servers different from normal A large number of failed DNS requests 
For example: 
google.com 
researchgate.com 
medium.com
 may be normal-looking queries. 
In contrast: 
a8dlae1k2d91.example.com xjdqd81jd82kd.example.com pmaak291jljwk.example.com 
a large number of unusual queries may require more detailed examination. A long or random domain alone does not necessarily mean it is malicious. When performing a security analysis, context, frequency, target, and other logs should be considered together.

In summary DNS is a building block that plays a key role on the internet. DNS general function is to turn domain names into IP addresses. To make DNS safer and give protection DNS can use tools such, as DNSSEC, DoH and DoT.
