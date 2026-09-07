---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 5b.co
  spf: true
hosts:
- cert_expires: Nov 23 01:06:08 2026 GMT
  host: 5b.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 5B4844 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 5B Australia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 5B Australia
provider_slug: 5b4844
slug: 5b4844-domain-security
source_filename: 5b4844-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 5b.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 01:06:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 5b.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/5b4844/refs/heads/main/security/5b4844-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Solar
- Renewable Energy
- Cleantech
- Energy
- Manufacturing
- Hardware
- Utility Scale Solar
- Mining
- Australia
- Company
---
