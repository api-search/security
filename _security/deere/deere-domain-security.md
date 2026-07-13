---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deere.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.deere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: developer.deere.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Deere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for John Deere, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: John Deere
provider_slug: deere
slug: deere-domain-security
source_filename: deere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.deere.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deere/refs/heads/main/security/deere-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- Agricultural Technology
- AgTech
- Construction
- Farming
- Forestry
- Machinery
- Operations Center
- Precision Agriculture
- Fortune 100
---
