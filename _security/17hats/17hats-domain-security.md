---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 17hats.com
  spf: true
hosts:
- cert_expires: Oct  4 05:57:41 2026 GMT
  host: www.17hats.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 17Hats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 17hats, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 17hats
provider_slug: 17hats
slug: 17hats-domain-security
source_filename: 17hats-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.17hats.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:57:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 17hats.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/17hats/refs/heads/main/security/17hats-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Small Business
- Invoicing
- Scheduling
- Bookkeeping
- Workflow Automation
- Contract Management
- Payments
- SaaS
---
