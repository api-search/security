---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: storylane.io
  spf: true
hosts:
- cert_expires: Sep  7 09:17:21 2026 GMT
  host: www.storylane.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 11:28:22 2026 GMT
  host: docs.storylane.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: api.storylane.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Storylane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Storylane, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Storylane
provider_slug: storylane
slug: storylane-domain-security
source_filename: storylane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.storylane.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 09:17:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.storylane.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 11:28:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.storylane.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: storylane.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storylane/refs/heads/main/security/storylane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Interactive Demos
- Product Walkthroughs
- Sales Enablement
- Marketing
- Demo Analytics
- Demo Automation
- Buyer Hub
- Sales
---
