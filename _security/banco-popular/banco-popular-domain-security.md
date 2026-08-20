---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: popular.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: popularbank.com
  spf: true
hosts:
- cert_expires: Oct  2 01:21:47 2026 GMT
  host: www.popular.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:51:42 2026 GMT
  host: www.popularbank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Banco Popular Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Popular (Banco Popular), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Popular (Banco Popular)
provider_slug: banco-popular
slug: banco-popular-domain-security
source_filename: banco-popular-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.popular.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:21:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.popularbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:51:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: popular.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: popularbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banco-popular/refs/heads/main/security/banco-popular-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial-Services
- Banking
- United States
- Puerto Rico
- Regional Bank
- Open Finance
- Data Aggregation
---
