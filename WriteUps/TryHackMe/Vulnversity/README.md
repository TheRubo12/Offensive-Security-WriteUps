# Vulnversity — File upload bypass & systemctl SUID privesc

**Plataforma:** TryHackMe  
**Fecha:** 2026  
**Tags:** linux, web, file-upload, burp, rce, suid, systemctl

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- Service recon (21/22/139/445/3128/3333)
- Discover /internal upload form
- Burp Intruder extension bypass (.phtml)
- Reverse shell
- SUID systemctl abuse to root

## Hallazgos clave
- Weak file extension validation on upload
- Dangerous SUID on systemctl enabling service execution as root

## Mitigaciones / Hardening
- Strict server-side file validation; store uploads outside web root
- Remove SUID from systemctl; audit SUID binaries; least privilege

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
