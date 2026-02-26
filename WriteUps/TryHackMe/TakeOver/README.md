# TakeOver — Subdomain enumeration & SSL SAN disclosure (takeover risk)

**Plataforma:** TryHackMe  
**Fecha:** 2026  
**Tags:** osint, vhost, ssl, san, subdomain-takeover, cloud

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- VHOST enumeration
- SSL certificate SAN analysis
- Hidden subdomain discovery
- Cloud endpoint misconfiguration risk

## Hallazgos clave
- Internal subdomains disclosed via certificate SAN
- Potential dangling DNS / cloud resource (takeover risk)

## Mitigaciones / Hardening
- Inventory subdomains; remove unused DNS records
- Avoid leaking internal names in public certs when possible
- Monitor for dangling DNS; validate cloud resources ownership

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
