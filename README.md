<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>

<h1>Nmap Demonstration</h1>

<h2>Description:</h2>
<p>Nmap (Network Mapper) is a powerful open-source network scanning tool used for discovering hosts and services on a computer network, thus creating a "map" of the network's topology. It offers a wide range of features for network reconnaissance, security auditing, and vulnerability assessment.</p>

<h2>Ownership Statement:</h2>
This project and all associated files are the original work of ByteBanterDK. If you use any part of this project, please ensure you comply with the applicable laws and regulations in your jurisdiction, including but not limited to copyright laws in the United Kingdom. For any enquiries or collaboration opportunities, please contact me at DenisKTechnology@protonmail.com.

<h2>Key Objectives:</h2>
<ul>
    <li>Perform network scans to identify active hosts and open ports.</li>
    <li>Conduct OS detection to determine the operating systems of target hosts.</li>
    <li>Explore various scanning techniques and Nmap options to gather comprehensive network information.</li>
    <li>Utilise Nmap's scripting engine for vulnerability detection and service enumeration.</li>
    <li>Understand the importance of root access in executing certain Nmap commands effectively.</li>
</ul>

<h2>Utilities Used:</h2>
<ul>
    <li>Nmap: The primary tool for network scanning and reconnaissance.</li>
    <li>Kali Linux Terminal: Provides an environment for executing Nmap commands.</li>
    <li>Windows OS: Target machine for network scans.</li>
</ul>

<h2>Environments Used:</h2>
<ul>
    <li>Operating Systems: Kali Linux, Windows</li>
    <li>Hardware: Virtual Machines</li>
    <li>Tools: Nmap, Terminal</li>
</ul>

<h2>Programme Walk-through:</h2>

<h3>Login as Root:</h3>
<img src="https://i.imgur.com/1DsWp0p.png" alt="Root Access Screenshot">
<p>Root access is essential when using Nmap or the Kali Linux terminal because many Nmap commands require elevated privileges to access and manipulate network resources effectively. In the screenshot, we're using a Windows OS on a VirtualBox to scan the computer's IP address.</p>

<h3>Finding Windows Machine IP Address:</h3>
<p>Use the <code>ipconfig</code> command on the Windows machine to determine its IP address.</p>
<img src="https://github.com/user-attachments/assets/46d5d7e7-4776-449b-8b84-846fb41c0535" alt="Finding IP Address Screenshot">

<h3>Executing Nmap Commands:</h3>
<img src="https://github.com/user-attachments/assets/fb5391fa-3512-4db7-8eb9-b18139d2b874" alt="Executing Nmap Commands Screenshot">
<p><code>nmap -O -d -v TARGET</code>: Performs aggressive OS detection with debugging and verbose output on the target IP address <code>TARGET</code>.</p>
<img src="https://github.com/user-attachments/assets/4e1ed816-4867-4d35-b0c7-0f36d6d0fe37" alt="Nmap Command Screenshot">
<p><code>nmap -Sp TARGET/24</code>: Conducts a ping scan on the specified subnet to identify responsive hosts.</p>
<img src="https://github.com/user-attachments/assets/f9ba0c67-4ad6-4a21-9220-19cda859800b" alt="Ping Scan Screenshot">
<img src="https://github.com/user-attachments/assets/6480e7aa-5911-4dac-833c-7fc27d46783d" alt="Nmap Command Screenshot">
<p><code>nmap -sS TARGET</code>: Initiates a SYN scan to determine open ports on the target system.</p>
<img src="https://github.com/user-attachments/assets/3d825263-2bb4-443f-809c-ce265048525a" alt="SYN Scan Screenshot">
<p><code>nmap --script vuln TARGET</code>: Utilises Nmap's scripting engine to perform vulnerability detection on the target.</p>
<img src="https://github.com/user-attachments/assets/e4959a48-c4fc-40b2-8829-1b3782105ceb" alt="Vulnerability Detection Screenshot">

<h3>Basic Nmap Commands:</h3>
<ul>
    <li><code>nmap -sP &lt;target&gt;</code>: Ping scan to check which hosts are up.</li>
    <li><code>nmap -sV &lt;target&gt;</code>: Version detection scan to determine service versions.</li>
    <li><code>nmap -A &lt;target&gt;</code>: Aggressive scan with OS detection, version detection, script scanning, and traceroute.</li>
</ul>

<h3>Advanced Nmap Commands:</h3>
<ul>
    <li><code>nmap -p 1-65535 &lt;target&gt;</code>: Scan all ports on the target.</li>
    <li><code>nmap -T4 -A -v &lt;target&gt;</code>: Aggressive scan with timing template 4 for faster execution.</li>
    <li><code>nmap -O &lt;target&gt;</code>: Enable OS detection.</li>
    <li><code>nmap -sU &lt;target&gt;</code>: Scan for open UDP ports.</li>
    <li><code>nmap -Pn &lt;target&gt;</code>: Skip host discovery and treat all hosts as online.</li>
</ul>

<h2>Outro</h2>

<h3>Conclusion</h3>
<p>In this demonstration, we explored the capabilities of Nmap as a powerful network scanning tool. We performed various scans to identify active hosts, open ports, and potential vulnerabilities on a target Windows machine. By utilising different Nmap commands and techniques, we gained valuable insights into the network's structure and security posture.</p>

<h3>Lessons Learned</h3>
<p>This project highlighted the importance of network reconnaissance in identifying security weaknesses. I learned how to effectively use Nmap's features to gather comprehensive information about networked devices and services, which is essential for any cybersecurity professional.</p>

<h3>Future Work</h3>
<p>Moving forward, I plan to delve deeper into Nmap's scripting engine to automate vulnerability assessments and explore additional scanning techniques. I will also investigate how to integrate Nmap with other security tools for enhanced network monitoring and analysis, ensuring a more robust security posture.</p>

<h3>Get in Touch</h3>
<p>If you have any questions about this demonstration or would like to collaborate on future projects, feel free to reach out! I am always open to discussions and knowledge sharing in the field of cybersecurity.</p>
<img align="left" alt="ByteBanterDK | Gmail" width="22px" src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fcdn-1.webcatalog.io%2Fcatalog%2Fprotonmail%2Fprotonmail-icon.png&f=1&nofb=1&ipt=6df4d08d62fc42ad07c8ae70905a4a6c79ce00471af3644e6281517111e85d03&ipo=images"/>DenisKTechnology@protonmail.com

</body>
</html>
