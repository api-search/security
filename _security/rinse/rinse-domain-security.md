---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rinse.com
  spf: true
hosts:
- cert_expires: Aug 30 15:59:26 2026 GMT
  host: www.rinse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rinse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rinse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rinse
provider_slug: rinse
slug: rinse-domain-security
source_filename: rinse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rinse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:59:26 2026 GMT\n  hsts: false\ndomains:\n- domain: rinse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rinse/refs/heads/main/security/rinse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Laundry
- Dry Cleaning
- Delivery
- Logistics
- On-Demand
- Local Services
---
