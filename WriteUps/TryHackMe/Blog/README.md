# Blog — WordPress RCE + SUID Privilege Escalation

**Plataforma:** TryHackMe  
**Fecha:** 2026-02  
**Tags:** linux, wordpress, rce, suid, metasploit, ltrace

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- SMB share discovery
- WordPress user enumeration + password brute force
- Authenticated RCE (wp_crop_rce)
- SUID env/variable abuse to root

## Hallazgos clave
- Writable SMB share exposed content
- Weak WordPress credentials
- RCE via vulnerable WP component
- SUID binary unsafe use of environment variable

## Mitigaciones / Hardening
- Restrict SMB shares; enforce auth and least privilege
- Enforce strong WP passwords; lockout/rate limit
- Patch WP core/plugins; remove unused components
- Audit and remove dangerous SUID binaries; use absolute paths; sanitize env

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
