---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: greendot.com
  spf: true
hosts:
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.greendot.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 11:47:00 2026 GMT
  host: developer.greendot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.greendot.com
  https: false
kind: domain-security
layout: security
method: probed
name: Green Dot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Green Dot Corporation, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Green Dot Corporation
provider_slug: green-dot
slug: green-dot-domain-security
source_filename: green-dot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.greendot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.greendot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:47:00 2026 GMT\n  hsts: null\n- host: api.greendot.com\n  https: false\ndomains:\n- domain: greendot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/green-dot/refs/heads/main/security/green-dot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Prepaid Cards
- Banking
---
