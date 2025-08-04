# 📡 Domain Name System (DNS)

## 🌐 What is DNS?

The **Domain Name System (DNS)** acts like the internet's phonebook. It translates domain names (like `example.com`) into IP addresses (like `93.184.216.34`) so that browsers can load resources from those addresses.

---

## 🧠 How DNS Works (Step-by-Step)

1. **User Enters URL**  
   You type a URL like `www.example.com` in your browser.

2. **DNS Resolver (Recursive Resolver)**  
   The request goes to a DNS resolver (usually provided by your ISP).

3. **Root DNS Server**  
   The resolver asks the root server where to find `.com` domains.

4. **TLD Server (.com, .net, etc.)**  
   The root server responds with the address of the Top-Level Domain (TLD) server for `.com`.

5. **Authoritative DNS Server**  
   The TLD server points to the domain’s authoritative DNS server.

6. **IP Address Returned**  
   The authoritative server responds with the actual IP address.

7. **Website Loaded**  
   The browser uses the IP to connect to the web server and load the website.

---

## 📁 Common DNS Record Types

| Record | Purpose                              |
|--------|--------------------------------------|
| A      | Maps a domain to an IPv4 address     |
| AAAA   | Maps a domain to an IPv6 address     |
| CNAME  | Alias of one domain to another       |
| MX     | Mail exchange record for email       |
| TXT    | Holds text (often for SPF, DKIM, etc)|
| NS     | Specifies authoritative nameservers  |
| PTR    | Maps IP to domain (reverse lookup)   |

---

## 🛠️ Useful DNS Tools

- `nslookup`
- `dig`
- `host`
- `whois`
- Online tools:
  - [DNSDumpster](https://dnsdumpster.com)
  - [ViewDNS](https://viewdns.info)
  - [MXToolbox](https://mxtoolbox.com)

---

## 🔐 DNS in Cybersecurity

- **DNS Enumeration**  
  Used in reconnaissance to find subdomains or hidden infrastructure.  
  Tools: `Amass`, `Sublist3r`, `dnsenum`

- **DNS Spoofing / Poisoning**  
  Attackers corrupt DNS cache to redirect users to malicious sites.

- **DNS Tunneling**  
  Technique to exfiltrate data over DNS queries.  
  Tools: `iodine`, `dnscat2`

---

## 📚 References

- [Cloudflare - What is DNS?](https://www.cloudflare.com/learning/dns/what-is-dns/)
- [OWASP - DNS Security](https://owasp.org/www-community/attacks/DNS_Rebinding)
- [`dig` command manual](https://linux.die.net/man/1/dig)

