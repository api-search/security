---
certifications:
- SOC 2 Type 2
description: ''
kind: trust-center
layout: security
name: Stensul Trust Center
name_suffix: Trust Center
overview: Stensul maintains a public trust center documenting SOC 2 Type 2 compliance.
provider_name: Stensul
provider_slug: stensul
slug: stensul-trust-center
source_filename: stensul-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://stensul.com/security-trust-center/\nname: Stensul Trust Center\ntrust_center:\n  url: https://trust.stensul.com/\n  platform: Vanta\n  platform_evidence: >-\n    trust.stensul.com is a CNAME to 69125d98e3c54bf4327d5701.cname.vantatrust.com.\n    The page is a client-side single-page application; the served HTML is a\n    5,435-byte shell, so certification detail below is read from Stensul's own\n    server-rendered security page rather than from the SPA.\n  http_status: 200\nsecurity_page:\n  url: https://stensul.com/security-trust-center/\n  http_status: 200\ncertifications:\n- name: SOC 2 Type 2\n  status: certified\n  evidence: >-\n    \"Audited annually by and complies with the AICPA standards for Controls at a\n    Service Organization\" — https://stensul.com/security-trust-center/\n  scope: annual\nnot_claimed:\n- ISO 27001\n- PCI DSS\n- HIPAA\n- FedRAMP\n- TX-RAMP\nnot_claimed_note: >-\n  None of these appear\
  \ on Stensul's public security page or in any public\n  Stensul material found during this pass. Absence here means \"not published\",\n  not \"not held\".\ncontrols_published:\n- area: authentication\n  detail: SSO via OAuth 2.0 / OpenID Connect and SAML 2.0\n- area: encryption\n  detail: TLS/HTTPS in transit with 2048-bit keys; encryption at rest\n- area: infrastructure\n  detail: Hosted on Google Cloud Platform and Amazon Web Services\n- area: network\n  detail: Globally distributed DDoS protection; intrusion detection system (IDS)\n- area: access\n  detail: Two-factor authentication required for server access\n- area: personnel\n  detail: Mandatory employee security training\nnotes: >-\n  Stensul publishes a certification posture and a control summary but no\n  vulnerability disclosure policy, no security.txt on its own apex, and no bug\n  bounty program — see security/stensul-vulnerability-disclosure.yml for that\n  negative result.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stensul/refs/heads/main/security/stensul-trust-center.yml
summary_line: SOC 2 Type 2
tags:
- Company
- Email
- Email Marketing
- Marketing
- Marketing Automation
- Content Management
- Landing Pages
- Marketing Operations
- Enterprise Software
- Governance
- Collaboration
- Software-as-a-Service
trust_url: ''
---
