---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daerogroup.com
  spf: true
hosts:
- cert_expires: Aug 20 11:41:57 2026 GMT
  host: www.daerogroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daero Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daero Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Daero Group
provider_slug: daero-group
slug: daero-group-domain-security
source_filename: daero-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.daerogroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 11:41:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: daerogroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daero-group/refs/heads/main/security/daero-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Construction Technology
- Field Operations
- Field Service Management
- Mobile
- Voice
- Project Management
- Trades
---
