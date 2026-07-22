---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: remoovit.com
  spf: true
hosts:
- cert_expires: Oct 15 07:46:49 2026 GMT
  host: remoovit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Remoov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remoov, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Remoov
provider_slug: remoov
slug: remoov-domain-security
source_filename: remoov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: remoovit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 07:46:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: remoovit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remoov/refs/heads/main/security/remoov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Junk Removal
- Furniture Resale
- Consignment
- Recycling
- Donation
- Home Services
- Decluttering
- Moving
- Sustainability
---
