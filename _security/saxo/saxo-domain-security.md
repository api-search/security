---
api_specs:
- filename: trade.yaml
  format: yaml
  label: Saxo Bank OpenAPI
  slug: saxo-bank-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saxo/refs/heads/main/openapi/trade.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: developer.saxo
  spf: true
- caa:
  - 0 issue "letsencrypt.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:dnsmaster@saxobank.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saxobank.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.developer.saxo
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: gateway.saxobank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.home.saxo
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saxo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saxo Bank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Saxo Bank
provider_slug: saxo
slug: saxo-domain-security
source_filename: saxo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.developer.saxo\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\n- host: gateway.saxobank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\n- host: www.home.saxo\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: developer.saxo\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: saxobank.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:dnsmaster@saxobank.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saxo/refs/heads/main/security/saxo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Investment Banking
- Trading
- Equities
- Forex
- Options
- Futures
- Market Data
- Portfolio Management
- Orders
- Financial
---
