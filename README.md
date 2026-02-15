# WiFi-Security

rockyou.txt
import kagglehub

# Download latest version
path = kagglehub.dataset_download("wjburns/common-password-list-rockyoutxt")

print("Path to dataset files:", path)

# Project Description

Wi-Fi (IEEE 802.11) Security – Handshake Capture & Password Cracking Analysis

This project focuses on analyzing the security of Wi-Fi networks based on the IEEE 802.11 standard, with particular emphasis on WPA/WPA2 authentication mechanisms. The main objective was to understand how wireless security protocols operate and to demonstrate how weak passwords can compromise network security.

# Project Overview

Wireless networks are inherently vulnerable because communication occurs over radio waves, which can be intercepted. Over time, several security protocols have been introduced:

WEP – Weak and easily broken

WPA – Improved security using TKIP

WPA2 – Strong encryption with AES

WPA3 – Enhanced protection against offline attacks

Despite encryption improvements, weak passwords remain a critical vulnerability.

# Project Objective

The project aimed to:

Understand how WPA/WPA2 authentication works

Capture a WPA handshake from a controlled test (fake) Wi-Fi network

Perform a dictionary-based password attack using a wordlist

Evaluate how password strength affects security

# Tools Used

Hotspot – To create a test Wi-Fi network

Wireshark – To capture and analyze network traffic

Aircrack-ng – To analyze the WPA handshake and attempt password cracking

Rockyou.txt – Wordlist for dictionary attack

Capture file (.cap) – Contains the recorded WPA handshake

Windows 11 & macOS – Operating environments

# Methodology

A fake access point was created with a predefined password.

A connection attempt was made to trigger the WPA handshake.

Wireshark was used to capture the handshake traffic.

The captured .cap file was analyzed using Aircrack-ng.

A dictionary attack was performed using the Rockyou wordlist.

# Results

The WPA handshake was successfully captured.

Aircrack-ng initiated password testing using the wordlist.

The password “biscotte” was successfully discovered.

This demonstrated that even WPA/WPA2 encryption can be compromised if weak passwords are used.

# Challenges

Windows does not natively support monitor mode.

Correct file paths and formatting were required for Aircrack-ng.

The success of the attack depended heavily on the quality of the wordlist.

# Conclusion

The project highlights that Wi-Fi encryption alone does not guarantee security. Weak passwords significantly reduce protection, even under WPA2. The findings reinforce the importance of:

Using strong, complex passwords

Enabling WPA3 when available

Avoiding unsecured public networks or using a VPN
