<h1 align="center">Shaquille Johnson's GitHub Profile</h1>

## Welcome

Welcome to my GitHub! I'm **Shaquille Johnson**, an Associate CISO with a focus on offensive security, defense strategies, and cyber intelligence. My passion lies in building secure environments that not only defend but proactively anticipate and neutralize threats. With a firm belief in advancing the state of cybersecurity, I aim to merge cutting-edge tools and methodologies to bolster the safety and resilience of digital infrastructures.

## Core Expertise

### Offensive Security
Utilizing offensive tactics, I specialize in vulnerability assessments, penetration testing, and red team operations. By simulating real-world attack scenarios, I ensure that systems are robust enough to withstand modern adversarial techniques.

### Defensive Security
My defense strategies revolve around building resilient, scalable infrastructures with advanced detection mechanisms. From firewalls to encryption, I fortify networks by implementing multi-layered security measures designed to protect against evolving threats.

### Cyber Intelligence
Leveraging cyber intelligence, I focus on identifying, tracking, and mitigating threats through real-time data analysis. This includes harnessing threat intelligence platforms and using predictive analytics to stay ahead of attackers.

### Automation and Security Orchestration
Efficiency is key in both offense and defense. Through Python scripting and automation, I streamline security operations, minimizing human error and accelerating incident response.

## Certifications
- Associate CISO (EC-Council)
- CompTIA Security+

## Featured Projects

### Offensive Security Automation
A collection of Python scripts aimed at automating penetration testing, vulnerability scanning, and other offensive operations.

#### Sample Python Code
```python
import subprocess

# Automate a vulnerability scan using Nmap
def scan_vulnerabilities(target):
    result = subprocess.run(['nmap', '-sV', '--script=vuln', target], capture_output=True, text=True)
    print(result.stdout)

# Target system to scan
target_ip = '192.168.1.100'

# Run the vulnerability scan
scan_vulnerabilities(target_ip)

Defensive Security Scripts

Tools and scripts focused on defensive measures such as log analysis, firewall rule automation, and intrusion detection.

Sample Python Code

import os
import re

# Log analysis to detect brute-force attempts
def analyze_logs(logfile):
    brute_force_pattern = re.compile(r'failed password|authentication failure')
    with open(logfile, 'r') as f:
        for line in f:
            if brute_force_pattern.search(line):
                print(f'Brute force attempt detected: {line.strip()}')

# Analyze SSH logs
analyze_logs('/var/log/auth.log')

Cyber Intelligence Gathering

Scripts and tools to gather cyber intelligence, automate reconnaissance, and monitor threat landscapes in real-time.

Sample Python Code

import requests
import json

# Gather threat intelligence from an open API
def get_threat_intelligence(api_url):
    response = requests.get(api_url)
    if response.status_code == 200:
        data = json.loads(response.text)
        for threat in data['threats']:
            print(f"Threat: {threat['name']}, Severity: {threat['severity']}")
    else:
        print(f"Error: Unable to fetch data from {api_url}")

# Threat intelligence API endpoint
api_url = 'https://api.threatintel.com/v1/threats'

# Fetch and display threat intelligence
get_threat_intelligence(api_url)

How to Get Started

	1.	Clone the Repository:

git clone https://github.com/yourusername/cyber-security-ops.git
cd cyber-security-ops


	2.	Install Dependencies:
Ensure you have Python 3.x installed along with the required libraries. Install dependencies using:

pip install -r requirements.txt


	3.	Run the Scripts:
Each folder contains scripts for specific security operations (offense, defense, intelligence). Navigate to the respective directory and execute the scripts.
	4.	Explore the Notebooks:
Detailed Jupyter notebooks are provided for an in-depth analysis of the methodologies and tools used in each security domain.

Contributions

I welcome contributions from fellow security enthusiasts. Feel free to submit pull requests, suggest improvements, or raise issues if you find any. Together, we can enhance these tools and create a safer digital world.

License

This repository is licensed under the MIT License. Please see the LICENSE file for details.

Contact

For collaboration opportunities or inquiries, please contact me at Shaquilleajohnson@outlook.com. Let’s work together to secure the future!
