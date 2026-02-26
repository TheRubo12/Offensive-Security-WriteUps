# Brooklyn Nine Nine — FTP exposure + SSH bruteforce + sudo less privesc

**Plataforma:** TryHackMe  
**Fecha:** 2025  
**Tags:** linux, ftp, ssh, hydra, sudo, gtfobins

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- Anonymous FTP note disclosure
- SSH brute force for user creds
- sudo -l reveals less NOPASSWD
- GTFOBins less to root

## Hallazgos clave
- Anonymous FTP enabled
- Weak SSH password
- Over-permissive sudo rule (less)

## Mitigaciones / Hardening
- Disable anonymous FTP; permission hardening
- Rate-limit SSH; strong passwords/MFA
- Review sudoers; remove NOPASSWD for interactive programs

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
