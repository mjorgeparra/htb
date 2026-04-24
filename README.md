A fully self-contained, offline-ready HTML reference guide for HackTheBox — structured as a zero-to-hero learning path from absolute beginner through to Advanced Active Directory and binary exploitation.
→ Open the Guide · Screenshots · What's Inside · Who Is This For
</div>

⚡ Quick Start
bash# Clone the repo
git clone https://github.com/yourusername/htb-guide.git
cd htb-guide

# Open in browser — no server required, no dependencies
open htb-guide-v7.html          # macOS
xdg-open htb-guide-v7.html     # Linux
start htb-guide-v7.html         # Windows
That's it. One HTML file, zero dependencies, works fully offline.

What's Inside
The guide is split into 24 sections across a beginner → advanced progression. Every section has sub-tabs with targeted commands, annotated output, and copy buttons on every code block.
🟢 Beginner Track — Start Here
SectionWhat You'll Learn★ Start Here6-week learning roadmap, environment setup checklist, 9 common beginner mistakes to avoidLinux BasicsCLI navigation, file permissions, users/processes, bash scripting, network commands + interactive quizNetworkingTCP/UDP, IP addressing, HTTP request/response (annotated), reading nmap output line by lineGlossary40+ terms explained in plain English — RCE, LFI, SUID, privesc, foothold, AD, Kerberos and moreCTF 101What CTFs are, 8 challenge categories with tools, step-by-step first flag walkthrough, platform comparison
🟡 Intermediate
SectionWhat You'll LearnHTB OverviewVPN setup, difficulty tiers, Pwnbox, 30 recommended machines with difficulty ratingsMethodology7-phase kill chain (recon → flags), Windows and Linux post-exploitation commandsTools40+ tools across 6 sub-tabs: Recon, Web, Exploitation, PrivEsc, Password Cracking, File TransferWeb Attacks13 attack types: SQLi, LFI, file upload, command injection, SSRF, SSTI, NoSQLi, XXE, GraphQL, deserialization, HTTP smuggling, OAuth/JWTPriv EscLinux (sudo, SUID, cron, capabilities, shared libs), Windows (Potato, AlwaysInstallElevated, service perms), Kernel CVEs, Container EscapeShells & PayloadsEvery reverse shell language, full TTY upgrade methods, msfvenom recipes, web shells, port forwardingServices Deep DiveSMB, MSSQL/MySQL, Redis/MongoDB, SMTP/Mail, SNMP/NFS, Tomcat/Jenkins — full attack chains
🔴 Advanced
SectionWhat You'll LearnActive DirectoryASREPRoast, Kerberoast, PtH/PtT, DCSync, Golden Ticket, ACL abuse, BloodHound, ADCS (ESC1/ESC8), Delegation (unconstrained, constrained, RBCD)PivotingSSH tunneling (-L/-R/-D), Chisel, Ligolo-ng with TUN interface, Proxychains, multi-hop double pivotBuffer OverflowWindows x86 OSCP-style 6-step method, Linux x64 with pwntools, ret2libc, ROP chains, memory diagramsAV EvasionAMSI bypass techniques, AMSI patch, shellcode loaders in C, LOLBins, PowerShell policy bypassPersistenceLinux (SSH keys, cron, systemd, SUID bash), Windows (registry, scheduled tasks, RDP enable)OSINT & ReconShodan/Censys/crt.sh, Google dorks, DNS zone transfers, GitHub secret hunting, credential OSINTCrypto & StegoSteganography tools, hash identification, encoding reference, password-protected file cracking
📚 Reference
SectionWhat's InsideWordlistsWordlist reference table, CeWL targeting, hashcat rules, interactive wordlist generator, username permutationCheatsheet24 port reference cards, 12 clickable command cards, machine progress tracker (30 classic HTB boxes)ReportingHTB writeup templates, OSCP-style vuln report template, note-taking tool comparison, folder setup scriptMindsetRabbit hole detection, enumeration discipline, pre-box checklist, skill progression roadmapResourcesCurated platform comparison, structured 7-step learning path, certification guidance

Features

🔍 Live search — Ctrl+K from anywhere, searches across all 24 sections instantly
📋 Copy buttons — every code block has a one-click copy button (145 total)
🧠 Interactive quiz — Linux fundamentals quiz with immediate feedback and explanations
🎯 Machine tracker — click to mark 30 classic HTB machines as owned, tracks % completion
⚡ Wordlist generator — enter company/product name → generates target-specific password list
🗺 Learning path cards — clickable week-by-week plan that jumps to the relevant section
📝 Annotated output — nmap results, HTTP responses, memory diagrams with inline explanations
📱 Responsive — works on desktop, tablet, and mobile


Screenshots

The guide uses an HTB-themed dark UI with green-on-black terminal aesthetics and animated matrix background.

<details>
<summary>Start Here — Beginner Roadmap</summary>
The default landing page shows a 6-week learning plan, environment setup checklist, and 9 common mistakes grid.
</details>
<details>
<summary>Cheatsheet — Port Reference + Command Cards</summary>
24 port cards each with attack vector hints. 12 command card panels — every command is clickable to copy.
</details>
<details>
<summary>Active Directory — ADCS & Delegation</summary>
Certipy ESC1/ESC8 chains, Shadow Credentials, unconstrained delegation TGT capture, RBCD full exploit chain.
</details>
<details>
<summary>Buffer Overflow — Stack Memory Diagram</summary>
Visual stack layout before/after overflow, 6-step Windows x86 exploit development, pwntools for Linux x64.
</details>

Who Is This For
You are...This guide...Complete beginner, never used LinuxStart at ★ Start Here, follow the 6-week planKnow Linux but new to HTBStart at HTB Overview, then MethodologySolving Easy machines, want structureUse Cheatsheet and Methodology as daily referenceStuck on Medium machinesDeep-dive Web Attacks, PrivEsc, ServicesPreparing for OSCPFocus on Buffer Overflow, Methodology, ReportingPracticing AD attacksWork through the full Active Directory sectionRunning team CTFsCTF 101, Crypto & Stego, OSINT sections

Who This Is NOT For
This guide is for legal, authorized practice only on:

HackTheBox machines (hackthebox.com)
TryHackMe rooms (tryhackme.com)
Deliberately vulnerable VMs you own
Systems you have explicit written authorization to test

Unauthorized access to computer systems is illegal everywhere. This guide exists to help you learn ethical offensive security — not to facilitate harm.

Project Structure
htb-guide/
│
├── htb-guide-v7.html     # The entire guide — open this in your browser
└── README.md             # This file
The entire guide is a single self-contained HTML file. No build process, no npm install, no server. All CSS, JavaScript, and content are inline.

Version History
VersionHighlightsv7.0Zero-to-hero rewrite — Linux basics, Networking, Glossary, CTF 101, interactive quiz, 6-week roadmap, beginner mistake guidev6.0Services deep-dive (SMB relay, MSSQL xp_cmdshell, Redis RCE, Jenkins), Reporting templates, QA passv5.0Pivoting (Ligolo-ng, Chisel, multi-hop), ADCS/ESC1/ESC8, Delegation (RBCD), Container escape (Docker socket, LXD, cgroup)v4.0Buffer Overflow (Windows x86 + Linux x64), AV Evasion, Persistence, OSINT, machine progress trackerv3.0Active Directory, Shells & Payloads, Crypto/Stego, live search, copy buttonsv2.0Web attacks, PrivEsc, Tools arsenal, file transfer referencev1.0Initial release — Methodology, basic tools, mindset

Contributing
Contributions welcome. If you spot:

A broken URL or outdated tool reference
A missing technique that keeps appearing on HTB machines
A clearer way to explain something for beginners
A bug in the JavaScript (search, quiz, tracker)

Open an issue or submit a PR. Please keep contributions within the scope of legal, educational offensive security practice.

Resources Referenced
ResourceURLPurposeGTFOBinsgtfobins.github.ioLinux sudo/SUID/capability abuse referenceLOLBASlolbas-project.github.ioWindows living-off-the-land binariesHackTricksbook.hacktricks.xyzComprehensive attack technique wikiPortSwigger Web Academyportswigger.net/web-securityBest free web hacking labsRevShellsrevshells.comReverse shell payload generatorCyberChefgchq.github.io/CyberChefData encoding/decoding/transformationSecListsgithub.com/danielmiessler/SecListsWordlist collectionExploit-DBexploit-db.comPublic exploit databaseIppSecyoutube.com/@ippsecHTB machine walkthroughsHTB Academyacademy.hackthebox.comStructured HTB learning path

License
MIT License — see LICENSE for details.
Free to use, share, and modify. If you build something with it, a star ⭐ is appreciated.

<div align="center">
hack the planet · legally · from zero to hero · never stop learning
Built for the HTB community · Not affiliated with HackTheBox
</div>
