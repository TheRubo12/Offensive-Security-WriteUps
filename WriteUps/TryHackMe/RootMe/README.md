# RootMe — File upload RCE & SUID python escalation

**Plataforma:** TryHackMe  
**Fecha:** 2026-02  
**Tags:** linux, web, file-upload, rce, suid, reverse-shell

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- Dir brute force (/panel, /uploads)
- File upload bypass to webshell
- Reverse shell as www-data
- SUID python2.7 abuse to root

## Hallazgos clave
- Unrestricted file upload leading to code execution
- SUID python interpreter allowing privilege escalation

## Mitigaciones / Hardening
- Implement strict allow-list validation + storage outside web root
- Disable/limit SUID; remove SUID from interpreters; least privilege

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
