---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: roomiapp.com
  spf: true
hosts:
- cert_expires: Oct  3 17:29:10 2026 GMT
  host: roomiapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roomi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Roomi
provider_slug: roomi
slug: roomi-domain-security
source_filename: roomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roomiapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:29:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: roomiapp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roomi/refs/heads/main/security/roomi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Real Estate
- Rentals
- Roommates
- Marketplace
- Mobile
---
