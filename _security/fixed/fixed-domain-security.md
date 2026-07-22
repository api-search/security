---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fixed.com.au
  spf: true
hosts:
- cert_expires: Sep  6 17:04:45 2026 GMT
  host: fixed.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fixed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fixed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fixed
provider_slug: fixed
slug: fixed-domain-security
source_filename: fixed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fixed.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:04:45 2026 GMT\n  hsts: false\ndomains:\n- domain: fixed.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixed/refs/heads/main/security/fixed-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Construction
- Facility Management
- Maintenance
- Childcare
- Australia
- Trades Services
---
