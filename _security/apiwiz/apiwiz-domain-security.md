---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apiwiz.io
  spf: true
hosts:
- cert_expires: Aug 28 20:57:52 2026 GMT
  host: www.apiwiz.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apiwiz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIwiz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: APIwiz
provider_slug: apiwiz
slug: apiwiz-domain-security
source_filename: apiwiz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apiwiz.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 20:57:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apiwiz.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiwiz/refs/heads/main/security/apiwiz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Design
- API Gateway
- API Governance
- API Lifecycle
- API Management
- API Monetization
- API Security
- Automation
- Low-Code
- Observability
- Platform
---
