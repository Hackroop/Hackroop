# Threat Analysis Report: North Korean Campaign Targeting Security Researchers

**Date:** September 7, 2023
**Author:** Clement Lecigne and Maddie Stone, Threat Analysis Group

## Executive Summary

Google's Threat Analysis Group (TAG) has uncovered an ongoing and concerning cyber campaign originating from North Korean threat actors targeting security researchers. This campaign bears striking similarities to a previous one publicly disclosed by TAG in January 2021. The attackers have been exploiting zero-day vulnerabilities and deploying malicious files to compromise researchers in the field of vulnerability research and development. Notably, at least one zero-day exploit has been actively used against security researchers in recent weeks. The affected vendor has been alerted, and a patch is in progress.

TAG is providing an early warning to the security research community about this campaign, emphasizing the continued threat posed by government-backed attackers and the need for increased vigilance among security professionals.

## Tactics and Techniques

### Social Engineering and Relationship Building

Similar to the previously reported campaign, North Korean threat actors are utilizing social media platforms such as X (formerly Twitter) to establish connections with their targets. They engage in prolonged conversations with researchers, attempting to build trust and collaboration. Once initial contact is established on social media, the threat actors transition to secure messaging apps like Signal, WhatsApp, or Wire. The goal is to develop a relationship that allows them to deliver malicious payloads effectively.

### Exploitation via Malicious Files

After establishing trust, the attackers send a malicious file containing one or more zero-day exploits for popular software packages. Upon successful exploitation, the malicious code conducts checks to identify virtual machine environments and exfiltrates information, including screenshots, to an attacker-controlled command and control server. The shellcode used in these exploits bears similarities to previous North Korean campaigns.

### Zero-Day Vulnerability Disclosure

TAG has reported the identified zero-day vulnerabilities to the affected vendor, who is actively working on patches. Once the vulnerabilities are patched, TAG will provide detailed technical information and analysis in accordance with their disclosure policies
