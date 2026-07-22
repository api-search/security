---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: armstrongceilings.com
  spf: true
hosts:
- cert_expires: Aug 21 16:14:00 2026 GMT
  host: www.armstrongceilings.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Armstrong World Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Armstrong World Industries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Armstrong World Industries
provider_slug: armstrong-world-industries
slug: armstrong-world-industries-domain-security
source_filename: armstrong-world-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.armstrongceilings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:14:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: armstrongceilings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armstrong-world-industries/refs/heads/main/security/armstrong-world-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Architecture
- Building Materials
- Ceilings
- Construction
- Manufacturing
- Walls
- Fortune 1000
---
