<h1 align="center"><b>PORT SCANNER PROJECT – Beginner Python Networking Project</b></h1>

<h2>Project Overview</h2>

<p>
This project is a beginner friendly TCP port scanner written in Python programming language using built in socket module.
The scanner checks whether ports on a target machine are open or closed by attempting real TCP connections.
</p>

<h2>This Project Helps To Understand</h2>

<ul>
<li>TCP/IP networking</li>
<li>Sockets</li>
<li>Port communication</li>
<li>Active scanning</li>
<li>Linux networking basics</li>
<li>Cybersecurity fundamentals</li>
</ul>

<h2>Project Goal</h2>

<ol>
<li>Learn Python networking</li>
<li>Understand TCP communication</li>
<li>Learn how port scanning works</li>
<li>Simplified version of Nmap relevant to Nmap -sT</li>
</ol>

<h2>What Is Port Scanning?</h2>

<p>
Port scanning is the process of checking network ports on a device to determine:
</p>

<ol>
<li>Which service is running</li>
<li>Which ports are up</li>
<li>Whether the host is reachable or not</li>
</ol>

<p>
Each network provides services which uses port numbers.
</p>

<p>
Note: Port number is nothing but the type of service for instance 21 – FTP, 22 – SSH, 80 – HTTP.
Open port means service is going on and it is in active state.
</p>

<h2>Type Of Scan Used</h2>

<p>
This project uses TCP Connect Scan.
</p>

<ol>
<li>Creates a TCP socket</li>
<li>Attempts for a TCP connection</li>
<li>Detects whether the connection succeeds</li>
</ol>

<h2>Technologies Used</h2>

<ul>
<li>Python3 – latest version of Python programming language</li>
<li>Socket module – Network module in Python</li>
<li>TCP/IP – Network transport protocol</li>
<li>Linux – for running the code</li>
</ul>

<h2>Concepts Learned</h2>

<ul>
<li>Python sockets</li>
<li>TCP handshake</li>
<li>IP addressing</li>
<li>Port communication</li>
<li>Client-Server networking</li>
<li>Active reconnaissance</li>
<li>Network scanning basics</li>
</ul>

<h2>TCP Handshake</h2>

<p>
TCP is a connection-oriented protocol.
</p>

<h3>If Port Active</h3>

<pre>
Client            Server
  SYN   -------->
        <-------- SYN-ACK
  ACK   -------->
</pre>

<h3>If Port Down</h3>

<pre>
Client            Server
  SYN   -------->
        <-------- RST
</pre>

<p>
Note: By default, if port is open at server network it will respond with SYN-ACK packets.
</p>

<h2>Project Workflow</h2>

<p>
The scanner performs the following steps:
</p>

<ol>
<li>Accept target IP address</li>
<li>Loop through ports</li>
<li>Create TCP socket</li>
<li>Attempt connecting using connect_ex()</li>
<li>Print open ports</li>
<li>Close socket</li>
</ol>

<h2>How To Run</h2>

<h3>Step 1 – Install Python</h3>

<p>
I used Kali Linux which already had Python installed.
</p>

<pre>
python3 --version
</pre>

<p>
If not installed:
</p>

<pre>
sudo apt install python3
</pre>

<h3>Step 2 – Save Code As scanner.py</h3>

<h3>Step 3 – Run Program</h3>

<pre>
python3 scanner.py
</pre>

<h3>Example Output</h3>

<pre>
Enter Target IP: 127.0.0.1

[OPEN] Port 21
[OPEN] Port 22
[OPEN] Port 80
</pre>

<h2>Important Note</h2>

<p>
Do not perform scanning without proper consent of the target.
Suggested to work out this project in labs or on localhost systems.
</p>

<p>
It is active scanning, therefore the target can detect scans and firewall logs may be generated.
This project is educational and focuses on understanding networking fundamentals.
</p>

<h2>Current Limitations</h2>

<ol>
<li>Sequential scanning</li>
<li>Slower speed</li>
<li>No multithreading</li>
<li>No UDP scanning</li>
<li>No service fingerprinting</li>
</ol>

<h2>Future Possible Improvements</h2>

<ol>
<li>Multithreading</li>
<li>Service detection</li>
<li>Network scanning</li>
<li>GUI interface</li>
<li>UDP scanning</li>
<li>Save reports to JSON/CSV</li>
<li>Async scanning</li>
</ol>

<h2>References</h2>

<ol>
<li>Python socket documentation</li>
<li>TCP/IP Networking fundamentals</li>
<li>Nmap documentation</li>
<li>Linux networking concepts</li>
<li>RFC – 793 – TCP protocol specification</li>
</ol>
