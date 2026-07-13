---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sheetz.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: b2bgateway.net
  spf: true
hosts:
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: www.sheetz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  6 16:47:20 2026 GMT
  host: www.b2bgateway.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sheetz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sheetz, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sheetz
provider_slug: sheetz
slug: sheetz-domain-security
source_filename: sheetz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sheetz.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.b2bgateway.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:47:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sheetz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: b2bgateway.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sheetz/refs/heads/main/security/sheetz-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Convenience Store
- Energy
- Food Service
- Fortune 500
- Fuel
- Retail
---
