---
certifications:
- SOC 2
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Webz Trust Center
name_suffix: Trust Center
overview: Webz.io maintains a public trust center documenting SOC 2 and ISO 27001 compliance.
provider_name: Webz.io
provider_slug: webz
slug: webz-trust-center
source_filename: webz-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://webz.io/trust\nurl: https://webz.io/trust\nhttp_status: 200\nverified: '2026-08-27'\nname: Webz.io Trust Center\nsummary: >-\n  A published trust page naming two audited security certifications and two privacy regimes, with the\n  ISO certificate available as a downloadable PDF. It is a static marketing-hosted page rather than a\n  hosted trust-center product (no trust.webz.io — DNS does not resolve), and it carries no security\n  contact, no vulnerability-disclosure policy and no subprocessor list.\ncertifications:\n- name: SOC 2\n  status: audit completed\n  evidence: >-\n    \"successfully completed the SOC 2 audit, demonstrating commitment to the highest standards of\n    security, confidentiality, and data integrity\"\n  report_available: not stated on the page\n- name: ISO 27001\n  status: certified\n  evidence: Certificate linked from the page as a PDF, alongside an IQNET certificate.\ncompliance_programs:\n\
  - name: GDPR\n  evidence: Named on the trust page as a \"leading and rigorous data protection and privacy regulation\" Webz.io complies with.\n- name: CCPA\n  evidence: California Consumer Privacy Act referenced alongside GDPR.\nlinked_documents:\n- name: Terms & Conditions\n  url: https://webz.io/tos/\n- name: Privacy Policy\n  url: https://webz.io/privacy/\n- name: Dark Web Policy\n  url: https://webz.io/dark-web-policy/\n- name: Status Page\n  url: https://status.webz.io\ngaps:\n- No security contact or responsible-disclosure policy on the page.\n- No /.well-known/security.txt on any Webz.io host (all 404).\n- No public bug bounty program found on HackerOne, Bugcrowd or Intigriti.\n- No subprocessor list, no penetration-test attestation, no data-residency statement.\n- trust.webz.io does not resolve; the trust content lives on the WordPress marketing site.\nprobes:\n- url: https://webz.io/trust\n  status: 200\n- url: https://trust.webz.io\n  status: 0\n  note: connection failed — host\
  \ does not resolve\n- url: https://webz.io/security\n  status: 404\n- url: https://webz.io/compliance\n  status: 404\n- url: https://webz.io/gdpr\n  status: 404\n- url: https://webz.io/.well-known/security.txt\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webz/refs/heads/main/security/webz-trust-center.yml
summary_line: SOC 2, ISO 27001
tags:
- News Data
- Web Data
- Web Scraping
- Dark Web
- deep-web
- Cybersecurity
- Threat Intelligence
- Data Breach
- pii-monitoring
- OSINT
- reviews-data
- AI Training Data
- Media Monitoring
trust_url: https://webz.io/trust
---
