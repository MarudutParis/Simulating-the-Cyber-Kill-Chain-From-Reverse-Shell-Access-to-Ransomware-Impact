<h1>Simulating-the-Cyber-Kill-Chain-From-Reverse-Shell-Access-to-Ransomware-Impact</h1>

<h2>Overview</h2>
<p>
This project demonstrates a simulated cyber attack chain in a controlled lab environment, starting from reverse shell access, followed by payload staging and delivery using a web server, and ending with ransomware execution to showcase post-exploitation impact on a Windows target system.
</p>

<h2>Disclaimer</h2>
<p>
This project was conducted strictly in a controlled lab environment for educational purposes only.
</p>

<h2>Lab Environment</h2>
<ul>
  <li><strong>Attacker Machine:</strong> Kali Linux</li>
  <li><strong>Target Machine:</strong> Windows 10</li>
  <li><strong>Tools Used:</strong> Metasploit, Apache Web Server, Windows Command Line</li>
  <li><strong>Network Type:</strong> NAT + Host-only</li>
</ul>

<h2>Attack Flow</h2>

<h3>1. Lab Setup</h3>
<p>
Apache web server is initialized on Kali Linux to host payloads, enabling delivery to the target machine.
</p>

<h3>2. Reverse Shell Establishment</h3>
<p>
A reverse TCP connection is established from the Windows target to the attacker machine, providing remote shell access through Meterpreter.
</p>

<h3>3. Payload Staging</h3>
<p>
The malicious payload is placed in the Apache web directory (<code>/var/www/html</code>) to allow remote access via HTTP.
</p>

<h3>4. Payload Delivery</h3>
<p>
The target system accesses the hosted payload through a web browser, initiating the download of the executable file.
</p>

<h3>5. Payload Download on Target</h3>
<p>
The payload is successfully downloaded and stored on the target system, preparing for execution.
</p>

<h3>6. Payload Execution</h3>
<p>
The downloaded payload is executed on the target machine, enabling post-exploitation activities.
</p>

<h3>7. Ransomware Simulation Impact</h3>
<p>
A simulated ransomware payload is executed, displaying a ransom message and demonstrating the potential impact of a successful attack.
</p>

<h2>Key Learning Outcomes</h2>
<ul>
  <li>Understanding the full attack chain from initial access to impact</li>
  <li>Demonstrating payload delivery and execution techniques</li>
  <li>Simulating ransomware behavior in a controlled environment</li>
  <li>Highlighting the importance of user interaction in cyber attacks</li>
</ul>
