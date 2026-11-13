# FUTURE_CS_01 — Website Vulnerability Assessment Report

## Objective
Produce a clear, business-friendly assessment of common website security risks and practical remediation advice.

## Scope and authorization
Assess only a website you own or have explicit written permission to assess. Start with passive observation and browser developer tools. Do not attempt exploitation, authentication bypass, denial of service, credential testing, or intrusive scanning. If permission or scope is unclear, stop and ask the site owner.

## Tools named in the internship brief
- Browser DevTools
- OWASP ZAP in passive mode only
- Nmap only when the owner has explicitly approved the exact host and scan scope
- Canva or another document editor for the final report

## Suggested workflow
1. Record the site URL, owner/permission, date, and assessment scope.
2. Browse public pages normally; note HTTPS, redirects, cookie attributes, security headers, exposed information, and mixed content.
3. Use browser DevTools to inspect requests and response headers.
4. If authorized, use OWASP ZAP passive analysis. Do not switch to active scanning.
5. Record each observation with evidence, impact, risk level, and a fix.
6. Re-check the affected page after the owner applies fixes.
7. Export the report as PDF and commit the report (remove personal data and secrets first).

## Risk scale
- **High:** could expose sensitive data or materially compromise an account/system.
- **Medium:** meaningful weakness requiring specific conditions or user interaction.
- **Low:** limited impact or defense-in-depth improvement.
- **Informational:** observation with no demonstrated security impact.

Do not label a theoretical concern as a confirmed vulnerability. Distinguish *observed*, *not tested*, and *not applicable*.

## Deliverables
- `report/assessment-report-template.md`
- `evidence/README.md`
- Final PDF report (after an authorized target is assessed)

## Repository structure
```text
FUTURE_CS_01/
├── README.md
├── report/
│   └── assessment-report-template.md
└── evidence/
    └── README.md
```
