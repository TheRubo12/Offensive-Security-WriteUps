# Basic — SSH bruteforce & SUID (/usr/bin/env) privesc

**Plataforma:** Vulnyx  
**Fecha:** 2025-09-04  
**Tags:** linux, ssh, bruteforce, suid, gtfobins

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- SSH password brute force
- Local enumeration
- SUID env abuse to root

## Hallazgos clave
- Weak SSH password on user account
- SUID env misconfiguration

## Mitigaciones / Hardening
- Enforce strong passwords + MFA; lockout/rate limiting
- Remove unnecessary SUID; audit via CIS baselines

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
