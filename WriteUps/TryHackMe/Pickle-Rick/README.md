# Pickle Rick — Web enumeration & sudo privilege abuse

**Plataforma:** TryHackMe  
**Fecha:** 2026-02  
**Tags:** linux, web, credential-exposure, sudo, misconfiguration

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- Source code review for hints
- robots.txt disclosure
- Panel command execution
- sudo -l abuse to access protected files

## Hallazgos clave
- Credentials exposed in public resources
- Command execution available via admin panel
- Over-permissive sudo configuration

## Mitigaciones / Hardening
- Avoid secrets in code/robots.txt; use vaults/env vars
- Harden admin panels; restrict command execution
- Review sudoers; remove NOPASSWD where not required

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
