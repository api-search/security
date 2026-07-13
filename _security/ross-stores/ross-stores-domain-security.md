---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rossstores.com
  spf: true
hosts:
- cert_expires: Feb  4 23:33:44 2027 GMT
  host: www.rossstores.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: corporate.rossstores.com
  https: false
- cert_expires: Nov 13 20:32:20 2026 GMT
  host: partners.rossstores.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ross Stores Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ross Stores, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ross Stores
provider_slug: ross-stores
slug: ross-stores-domain-security
source_filename: ross-stores-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rossstores.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:33:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: corporate.rossstores.com\n  https: false\n- host: partners.rossstores.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 20:32:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rossstores.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ross-stores/refs/heads/main/security/ross-stores-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fashion
- Fortune 500
- Off-Price Retail
- Retail
- Supply Chain
---
