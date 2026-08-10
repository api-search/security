---
certifications:
- HITRUST CSF
- HIPAA
description: ''
kind: trust-center
layout: security
name: Recuro Health Trust Center
name_suffix: Trust Center
overview: Recuro Health maintains a public trust center documenting HITRUST CSF and HIPAA compliance.
provider_name: Recuro Health
provider_slug: recuro-health
slug: recuro-health-trust-center
source_filename: recuro-health-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nprobe: false\nnotes: >-\n  0-working/probe-security-programs.py found nothing (trust.recurohealth.com does not\n  resolve; /trust, /security and /compliance all return 404 on recurohealth.com). This\n  file was written from a hand-fetched page the probe's path list does not cover: Recuro\n  Health publishes its compliance posture at /hitrust/, not at a conventional trust-center\n  path. There is no trust portal, no downloadable audit report, and no subprocessor list.\nurl: https://recurohealth.com/hitrust/\ncertifications:\n- HITRUST CSF\n- HIPAA\nframeworks:\n- id: hitrust-csf\n  status: certified\n  scope: Recuro Health infrastructure, platform and services\n  source: https://recurohealth.com/hitrust/\n- id: hipaa\n  status: published-policy\n  source: https://recurohealth.com/hipaa-policy/\n- id: ccpa-cpra\n  status: published-policy\n  source: https://recurohealth.com/california/\nnot_found:\n- SOC 2\n- ISO 27001\n- PCI DSS\n-\
  \ FedRAMP\n- CSA STAR\ncontact:\n  route: Security Compliance Team, via https://recurohealth.com/contact/\n  security_email: null\n  note: >-\n    The HITRUST page directs questions to a \"Security Compliance Team\" but publishes no\n    direct address; no security@ or abuse@ address appears on any public page, and\n    /.well-known/security.txt returns 404.\ngaps:\n- No RFC 9116 security.txt on any host.\n- No vulnerability disclosure or bug bounty program found (/responsible-disclosure,\n    /vulnerability-disclosure, /security all 404).\n- No status page (recurohealth.statuspage.io redirects to Atlassian's marketing site,\n    identical to a nonexistent-subdomain control — a soft 404, not a status page).\n- No public subprocessor list or downloadable audit artifact.\nevidence:\n- source: https://recurohealth.com/hitrust/\n  http_status: 200\n  keywords:\n  - HITRUST Certified\n  - HITRUST Alliance\n  - HIPAA\n  - compliance\n  - Security Compliance Team\n- source: https://recurohealth.com/hipaa-policy/\n\
  \  http_status: 200\n- source: https://recurohealth.com/california/\n  http_status: 200\n- source: https://recurohealth.com/security\n  http_status: 404\n- source: https://recurohealth.com/trust\n  http_status: 404\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://recurohealth.com/hitrust/\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recuro-health/refs/heads/main/security/recuro-health-trust-center.yml
summary_line: HITRUST CSF, HIPAA
tags:
- Company
- Health
- Healthcare
- Telehealth
- Virtual Care
- Digital Health
- Behavioral Health
- Primary Care
- Employee Benefits
- Health Plans
- Identity
- OpenID Connect
trust_url: https://recurohealth.com/hitrust/
---
