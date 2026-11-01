<h1 align="center">Shisones</h1>

<h3 align="center">C2 development · Windows malware · exploit development</h3>

<p align="center">
  I build the implant, then write the detection notes for it. Most of my work is C2 infrastructure and Windows malware, with exploit development on the side.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Focus-C2_%26_malware-8B0000?style=flat-square" alt="Focus: C2 and malware" />
  <img src="https://img.shields.io/badge/Arch_Linux-1793D1?style=flat-square&logo=archlinux&logoColor=white" alt="Arch Linux" />
  <img src="https://img.shields.io/badge/Neovim-57A143?style=flat-square&logo=neovim&logoColor=white" alt="Neovim" />
  <img src="https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white" alt="C" />
  <img src="https://img.shields.io/badge/Windows-0078D6?style=flat-square&logo=windows&logoColor=white" alt="Windows" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Burp_Suite-FF6633?style=flat-square&logo=burpsuite&logoColor=white" alt="Burp Suite" />
</p>

## Focus

I work on C2 infrastructure and Windows malware. My C2 framework uses encrypted tasking, Windows evasion, and post-quantum crypto. On the malware side, I rebuilt the nine process injection techniques from Cyberwarfare Labs' CPIA course in Rust: classic injection, APC injection, section mapping, module stomping, process hollowing, doppelganging, transacted hollowing, herpaderping, and ghosting. Modules 01 to 05 have win32 and ntdll variants, plus detection notes and a MITRE T1055 mapping.

I also write exploit PoCs. Recent ones cover a Keycloak reset-credentials bypass leading to account takeover, a FreePBX SQL injection chained to root RCE, and an OliveTin command injection. Outside userland, I spend time on Windows kernel and driver bugs.

## Public repos

| Repo | Stack | What it is |
| --- | --- | --- |
| [CVE-2026-27626](https://github.com/Shisones/CVE-2026-27626) | Python | OliveTin OS command injection through `password`-typed arguments. CVSS 9.9, and root when OliveTin runs as root. |
| [CVE-2025-31161](https://github.com/Shisones/CVE-2025-31161) | Python | CrushFTP authentication bypass with a mangled AWS4-HMAC header. Unauthenticated impersonation of any user. |
| [MetabaseRCE_CVE-2023-38646](https://github.com/Shisones/MetabaseRCE_CVE-2023-38646) | Rust | Metabase pre-auth RCE PoC using the setup token from `/api/session/properties`. |
| [Hashbrown](https://github.com/Shisones/Hashbrown) | Rust | Hash cracker and brute forcer for CTFs. SHA-256, SHA-1, MD5, and SHA-512, parallelized with rayon. |
| [Waka](https://github.com/Shisones/Waka) | Rust | pacman/libalpm frontend inspired by nala. Reads `pacman.conf` directly, live download progress, transaction history, AUR packages. |

Dotfiles are in [Dotfiles](https://github.com/Shisones/Dotfiles).

## Background

Before consulting, I spent two and a half years as a lab assistant at Universitas Pendidikan Indonesia, leading the network and security assistant team and running live-fire exercises with C2 malware. I also did a SOC internship at PT SCADA Prima Cipta and ran infrastructure for the Dinamik 18 and 19 contests.

## Elsewhere

Most of my work is private. The repos above are what I can share.

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Shisones&theme=github_dark" alt="Shisones GitHub profile summary" />
</p>
