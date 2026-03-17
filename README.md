# Cybersecurity Research Notes

This repository contains my technical research and articles focused on malware development, Windows internals, credential access, privilege escalation, and detection engineering. The goal is to explore offensive techniques from a defensive perspective to improve understanding, detection, and mitigation strategies.

---

## 6. Thread Telemetry Desynchronization – Part 2
This article builds upon previous research on PEB manipulation and explores how attackers create desynchronization at the thread level. Instead of focusing only on process-level artifacts, this research analyzes how multiple telemetry layers can present inconsistent views of the same execution.

By combining techniques such as PEB spoofing, thread context manipulation, LOLBin chaining, stack spoofing, and indirect syscalls, attackers can generate conflicting telemetry across user-mode and kernel-level observations.

**Key topics:** thread-level telemetry analysis, PEB spoofing, thread context manipulation, stack spoofing, indirect syscalls, multi-layer telemetry desynchronization.

---

## 5. Malware Development 5: Event Tracing for Windows (ETW)
This article investigates ETW, a key telemetry mechanism used by EDR, SIEM, and antivirus tools. It covers ETW architecture, attack techniques, and defense strategies to maintain visibility in Windows systems.  

**Key topics:** ETW architecture, telemetry importance, manipulation techniques, attack examples, defensive considerations.

---

## 4. Malware Development 4: Exploring AMSI
This article explores the Anti-Malware Scan Interface (AMSI) in Windows and how attackers may evade it. Understanding AMSI helps strengthen defensive strategies and provides insights into malware detection mechanisms.  

**Key topics:** AMSI operation, bypass techniques, defensive strategy enhancement, application integration, experimental lessons.

---

## 3. Privilege Escalation and User Account Control (UAC)
This article examines Windows privilege escalation, focusing on bypassing User Account Control (UAC). It explains how attackers elevate privileges, exploit weak permissions or vulnerable applications, and bypass UAC protections.  

**Key topics:** privilege escalation fundamentals, security risks, UAC mechanisms, common UAC bypass techniques, defensive implications.

---

## 2. Exploring Windows Security: Lessons Learned from Credential Dumping Attempts
This research focuses on credential dumping in Windows, particularly LSASS memory and LSA secrets. It explores how authentication data is stored, privilege requirements, and practical challenges in extracting credentials.  

**Key topics:** LSASS overview, NTLM hashes, LSA secrets, user mode vs kernel mode, credential extraction challenges.

---

## 1. Malware Development with Defensive Perspective
This article explores malware development while maintaining a strong defensive mindset. It focuses on building a basic malware sample, turning it into a dropper, and evaluating detection mechanisms. The goal is to understand malware behavior and identify weaknesses from a defensive standpoint.  

**Key topics:** shellcode introduction, dropper creation, application whitelisting evaluation, incremental malware improvements.
