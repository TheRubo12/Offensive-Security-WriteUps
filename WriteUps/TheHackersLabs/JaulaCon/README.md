# JaulaCon — ShellShock (CVE-2014-6271) RCE

**Plataforma:** TheHackersLabs  
**Fecha:** 2025-09-05  
**Tags:** linux, cgi, shellshock, cve-2014-6271, rce

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- CGI endpoint discovery
- Header injection exploit
- Reverse shell acquisition
- SUID enumeration for further privesc

## Hallazgos clave
- ShellShock unpatched allowing RCE via HTTP headers
- Web user shell obtained

## Mitigaciones / Hardening
- Patch Bash; disable vulnerable CGI; WAF rules
- Least privilege on web user; harden SUID set

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
