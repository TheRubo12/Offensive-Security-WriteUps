# Blue — MS17-010 (EternalBlue) RCE

**Plataforma:** TryHackMe  
**Fecha:** 2025-09-05  
**Tags:** windows, smb, ms17-010, eternalblue, metasploit

## Resumen
Informe del laboratorio centrado en una cadena de compromiso completa: reconocimiento → enumeración → acceso inicial → post-explotación / escalada → impacto.

## Cadena de ataque (alto nivel)
- SMB service identification
- Vuln confirmation
- EternalBlue exploitation
- SYSTEM shell verification

## Hallazgos clave
- Unpatched SMBv1 vulnerable to MS17-010
- Remote code execution as SYSTEM

## Mitigaciones / Hardening
- Patch management; disable SMBv1
- Network segmentation; restrict 445
- Monitor exploitation attempts; IDS/EDR

## Evidencias
- PDF: `report.pdf`

## Disclaimer
Uso exclusivamente educativo en entornos controlados. No aplicar estas técnicas sin autorización explícita.
