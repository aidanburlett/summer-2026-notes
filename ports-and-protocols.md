# Common Ports and Protocols

A reference list of essential networking ports, what each protocol does, the security risks involved, and common example attacks.

---

## Port 22 – SSH
**What it does:**  
Secure Shell provides encrypted remote login and command execution on servers and network devices.

**Security risks:**  
- Brute-force login attempts  
- Weak or reused passwords  
- Misconfigured SSH keys  
- Outdated SSH versions

**Example attacks:**  
- SSH brute-force attacks  
- Credential stuffing  
- Man-in-the-middle attacks if host keys aren’t verified

---

## Port 80 – HTTP
**What it does:**  
Handles unencrypted web traffic between browsers and servers.

**Security risks:**  
- Traffic is sent in plaintext  
- Easy to intercept or modify  
- Vulnerable to injection attacks

**Example attacks:**  
- Man-in-the-middle (MITM)  
- Cross-site scripting (XSS)  
- SQL injection  
- Session hijacking

---

## Port 443 – HTTPS
**What it does:**  
Encrypted version of HTTP using TLS/SSL for secure web communication.

**Security risks:**  
- Misconfigured certificates  
- Outdated TLS versions  
- SSL stripping attacks

**Example attacks:**  
- TLS downgrade attacks  
- Certificate spoofing  
- HTTPS MITM (with compromised certificates)

---

## Port 53 – DNS
**What it does:**  
Translates domain names (like google.com) into IP addresses.

**Security risks:**  
- DNS responses can be spoofed  
- DNS traffic is often unencrypted  
- Attackers can redirect users to malicious sites

**Example attacks:**  
- DNS poisoning  
- DNS spoofing  
- DNS amplification (DDoS)

---

## Port 3389 – RDP
**What it does:**  
Remote Desktop Protocol allows remote GUI access to Windows systems.

**Security risks:**  
- Highly targeted by attackers  
- Weak passwords lead to easy compromise  
- Exposing RDP to the internet is dangerous

**Example attacks:**  
- RDP brute-force  
- Credential theft  
- Ransomware deployment after RDP compromise

---

## Port 445 – SMB
**What it does:**  
Server Message Block handles Windows file sharing, printer sharing, and network communication.

**Security risks:**  
- Historically vulnerable  
- Wormable exploits  
- Lateral movement inside networks

**Example attacks:**  
- EternalBlue (used by WannaCry)  
- SMB relay attacks  
- Pass-the-hash attacks

---

## Port 25 – SMTP
**What it does:**  
Simple Mail Transfer Protocol sends outbound email between servers.

**Security risks:**  
- Often lacks authentication  
- Can be abused for spam  
- Vulnerable to spoofing

**Example attacks:**  
- Email spoofing  
- Phishing campaigns  
- SMTP open relay abuse

---

## Port 110 – POP3
**What it does:**  
Retrieves email by downloading messages from the server to the client.

**Security risks:**  
- Often unencrypted  
- Credentials can be intercepted  
- Susceptible to MITM attacks

**Example attacks:**  
- Credential interception  
- Session hijacking  
- Email tampering

---

## Port 143 – IMAP
**What it does:**  
Retrieves and syncs email across devices while keeping messages on the server.

**Security risks:**  
- Unencrypted IMAP exposes credentials  
- Attackers can access entire mailboxes  
- Weak authentication

**Example attacks:**  
- IMAP brute-force  
- Credential theft  
- Unauthorized mailbox access