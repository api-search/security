---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mars.com
  spf: true
hosts:
- cert_expires: Jul 30 19:06:54 2026 GMT
  host: www.mars.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 05:04:19 2026 GMT
  host: developer.mars.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mars Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mars, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mars
provider_slug: mars
slug: mars-domain-security
source_filename: mars-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mars.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 30 19:06:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.mars.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 05:04:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mars.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mars/refs/heads/main/security/mars-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Confectionery
- Consumer Packaged Goods
- Food
- Pet Care
- Pet Food
- Veterinary
---
