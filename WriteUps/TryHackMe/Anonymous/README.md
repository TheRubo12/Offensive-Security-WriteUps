# Anonymous — Anonymous FTP abuse & cron privilege escalation

**Plataforma:** TryHackMe  
**Fecha:** 2025-09-04  
**Tags:** linux, ftp, cron, reverse-shell, suid, gtfobins

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- FTP anonymous access
- Cron job script overwrite
- SUID env abuse to root

## Hallazgos clave
- Anonymous FTP enabled
- Root cron executes writable script
- SUID env misconfiguration

## Mitigaciones / Hardening
- Disable anonymous FTP; permissions hardening
- Secure cron scripts ownership/permissions
- Audit SUID binaries; enforce least privilege

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
