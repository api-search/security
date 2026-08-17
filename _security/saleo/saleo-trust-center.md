---
certifications:
- SOC 2 Type 2
- ISO 27001
- GDPR
description: ''
kind: trust-center
layout: security
name: Saleo Trust Center
name_suffix: Trust Center
overview: Saleo maintains a public trust center documenting SOC 2 Type 2, ISO 27001, and GDPR compliance.
provider_name: Saleo
provider_slug: saleo
slug: saleo-trust-center
source_filename: saleo-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: true\nurl: https://trust.saleo.io/\nplatform: Vanta\nnote: >-\n  probe-security-programs.py recorded trust=none for this provider because the\n  Vanta trust centre renders client-side — the served HTML carries only the\n  <head>, so the keyword threshold in the probe cannot be met. The trust centre is\n  real: the document declares rel=canonical https://trust.saleo.io, <title>Saleo\n  Trust Center</title>, and loads Vanta's index-trust-report bundle from\n  assets.vanta.com. The certification list below therefore comes from Saleo's own\n  security page rather than from the trust centre body, which is not machine-readable.\ncertifications:\n- SOC 2 Type 2\n- ISO 27001\n- GDPR\ncertification_source: https://saleo.io/platform/security/\nsecurity_contact: security@saleo.com\nevidence:\n- source: https://trust.saleo.io/\n  http_status: 200\n  keywords: [Saleo Trust Center, vanta, Trust, Security, Compliance]\n  machine_readable:\
  \ false\n  reason: client-side rendered Vanta trust report; body is a <head>-only shell\n- source: https://saleo.io/platform/security/\n  http_status: 200\n  keywords: [SOC 2 Type 2, ISO 27001, GDPR, RBAC, security@saleo.com]\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://trust.saleo.io/\n  http_status: 200\n  content_type: text/html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saleo/refs/heads/main/security/saleo-trust-center.yml
summary_line: SOC 2 Type 2, ISO 27001, GDPR
tags:
- Company
- Sales Tech
- Demo Automation
- Sales Enablement
- Presales
- Go-To-Market
- AI Agents
- SCIM
- Identity Provisioning
- Single Sign-On
- Interactive Demos
- Product Tours
trust_url: https://trust.saleo.io/
---
