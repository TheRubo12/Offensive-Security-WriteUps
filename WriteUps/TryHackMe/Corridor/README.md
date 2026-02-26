# Corridor — IDOR via predictable MD5 object IDs

**Plataforma:** TryHackMe  
**Fecha:** 2025  
**Tags:** web, idor, access-control, md5, owasp

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- Identify hashed IDs in URLs
- Detect MD5 pattern (sequential integers)
- Enumerate out-of-range objects
- Access hidden resource

## Hallazgos clave
- Predictable object identifiers
- Missing authorization checks (IDOR)

## Mitigaciones / Hardening
- Enforce server-side authorization checks
- Use non-guessable IDs + access control
- Audit endpoints for IDOR per OWASP

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
