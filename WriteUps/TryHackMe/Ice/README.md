# Ice — Icecast (CVE-2004-1561) RCE & credential dumping

**Plataforma:** TryHackMe  
**Fecha:** 2025-09-06  
**Tags:** windows, icecast, cve-2004-1561, metasploit, credential-dumping, rdp

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- Icecast service discovery
- Metasploit RCE
- Kiwi/hashdump
- Enable RDP for persistence

## Hallazgos clave
- Vulnerable Icecast service allows RCE
- Credential dumping possible
- RDP enabled for persistence

## Mitigaciones / Hardening
- Patch/upgrade Icecast; remove exposed service
- Enable EDR; restrict admin tools
- Harden RDP; MFA; restrict network access

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
