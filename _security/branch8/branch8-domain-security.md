---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: branch8.com
  spf: true
hosts:
- cert_expires: Sep  8 10:16:56 2026 GMT
  host: branch8.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Branch8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Branch8, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Branch8
provider_slug: branch8
slug: branch8-domain-security
source_filename: branch8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: branch8.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 10:16:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: branch8.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/branch8/refs/heads/main/security/branch8-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-Commerce
- CRM
- CDP
- Managed Services
- Digital Operations
- Data Engineering
- AI Automation
- Asia-Pacific
---
