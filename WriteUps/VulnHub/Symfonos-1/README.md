# Symfonos 1 — SMB enum → WordPress LFI/RCE → SUID PATH hijacking

**Plataforma:** VulnHub  
**Fecha:** 2026  
**Tags:** linux, samba, wordpress, lfi, rce, suid, path-hijacking

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- SMB share discovery + weak password hint
- WordPress discovery and plugin enum
- mail-masta LFI to RCE
- SUID /opt/statuscheck PATH hijack (curl) to root

## Hallazgos clave
- Weak credential hygiene exposed via SMB
- Vulnerable WP plugin enabling LFI/RCE
- SUID binary calling non-absolute executable path

## Mitigaciones / Hardening
- Harden SMB shares; remove weak password hints
- Patch/replace vulnerable plugins; WAF
- Fix SUID binary: absolute paths; drop SUID; sanitize PATH

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
