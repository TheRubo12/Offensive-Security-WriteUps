# Mr Robot — WordPress compromise & SUID nmap escalation

**Plataforma:** TryHackMe  
**Fecha:** 2025-09-04  
**Tags:** linux, wordpress, credential-exposure, rce, suid, hash-cracking

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- Directory enumeration
- Credential disclosure (Base64 in license)
- WP login + template/plugin modification RCE
- Hash cracking for lateral
- SUID nmap to root

## Hallazgos clave
- Credentials exposed in public file
- Authenticated RCE via WP editing
- SUID nmap enabling root shell

## Mitigaciones / Hardening
- Remove sensitive files; secure backups
- Disable file editor in WP; least privilege roles
- Remove SUID from nmap; audit SUID binaries

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
