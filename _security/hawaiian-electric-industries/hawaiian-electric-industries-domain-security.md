---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hei.com
  spf: true
hosts:
- cert_expires: Oct  9 12:45:16 2026 GMT
  host: www.hei.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hawaiian Electric Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hawaiian Electric Industries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hawaiian Electric Industries
provider_slug: hawaiian-electric-industries
slug: hawaiian-electric-industries-domain-security
source_filename: hawaiian-electric-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hei.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:45:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hei.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hawaiian-electric-industries/refs/heads/main/security/hawaiian-electric-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Utilities
- Holding Company
- Hawaii
- Fortune 1000
---
