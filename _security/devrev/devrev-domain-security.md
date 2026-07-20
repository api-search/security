---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: devrev.ai
  spf: true
hosts:
- cert_expires: Oct 14 19:52:54 2026 GMT
  host: devrev.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 09:35:33 2026 GMT
  host: developer.devrev.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 21:44:25 2026 GMT
  host: api.devrev.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Devrev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Devrev, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Devrev
provider_slug: devrev
slug: devrev-domain-security
source_filename: devrev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devrev.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:52:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.devrev.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 09:35:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.devrev.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 21:44:25 2026 GMT\n  hsts: null\ndomains:\n- domain: devrev.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devrev/refs/heads/main/security/devrev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Support
- Product Development
- Issue Tracking
- Knowledge Base
- CRM
- Developer Tools
- AI
- Webhooks
- Automation
---
