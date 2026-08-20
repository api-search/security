---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: walnut.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: teamwalnut.com
  spf: false
hosts:
- cert_expires: Sep 18 06:03:58 2026 GMT
  host: www.walnut.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: help.walnut.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: customer-api.teamwalnut.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Walnut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Walnut, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Walnut
provider_slug: walnut
slug: walnut-domain-security
source_filename: walnut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.walnut.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 06:03:58 2026 GMT\n  hsts: false\n- host: help.walnut.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: customer-api.teamwalnut.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: walnut.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: teamwalnut.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/walnut/refs/heads/main/security/walnut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Sales Demo
- Interactive Demos
- Product Demos
- Sales Enablement
- Demo Analytics
- Go-To-Market
- AI-Powered
- Webhook
- MCP
- Analytics
---
