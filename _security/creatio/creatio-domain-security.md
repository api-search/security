---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: creatio.com
  spf: true
hosts:
- cert_expires: Sep 22 15:29:17 2026 GMT
  host: www.creatio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Creatio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creatio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Creatio
provider_slug: creatio
slug: creatio-domain-security
source_filename: creatio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.creatio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:29:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: creatio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creatio/refs/heads/main/security/creatio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Saas
- CRM
- No-Code
- Low-Code
- Business Process Management
- Workflow Automation
- Sales
- Marketing
- Customer Service
- OData
- AI Agents
---
