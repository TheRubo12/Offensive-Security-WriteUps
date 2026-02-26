# Startup — Anonymous FTP → PCAP credential leak → Cron privesc

**Plataforma:** TryHackMe  
**Fecha:** 2026  
**Tags:** linux, ftp, pcap, wireshark, cron, privilege-escalation

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- Anonymous FTP write access
- Web exposure of FTP directory
- PCAP analysis for credentials
- Cronjob/script abuse to root

## Hallazgos clave
- Anonymous FTP with write permissions
- Sensitive credentials leaked in captured traffic
- Root cron executing user-writable script

## Mitigaciones / Hardening
- Disable anonymous FTP; enforce auth and permissions
- Avoid storing/transporting creds in cleartext; use TLS
- Harden cron jobs; ensure root scripts are not writable by users

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
