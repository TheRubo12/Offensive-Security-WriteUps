# Easy Peasy — Multi-stage web enum + stego + SSH + cron privesc

**Plataforma:** TryHackMe  
**Fecha:** 2025  
**Tags:** linux, web, steganography, ssh, cron

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- Multi-port web enumeration
- Decode hidden strings (base/rot/binary)
- Stego extraction for creds
- SSH access
- Cron script abuse to root

## Hallazgos clave
- Sensitive info exposed in web content
- Credentials hidden in media
- Root cron executes unsafe script

## Mitigaciones / Hardening
- Remove secrets from web; secure media
- Strong credential policies; rotate
- Secure cron jobs; integrity checks

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
