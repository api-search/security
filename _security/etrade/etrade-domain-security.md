---
api_specs:
- filename: etrade-openapi.yml
  format: yaml
  label: E*TRADE API
  slug: etrade
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/etrade/refs/heads/main/openapi/etrade-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:domains@etrade.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: etrade.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: us.etrade.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: developer.etrade.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api.etrade.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Etrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Etrade, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Etrade
provider_slug: etrade
slug: etrade-domain-security
source_filename: etrade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: us.etrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.etrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: api.etrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: etrade.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:domains@etrade.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/etrade/refs/heads/main/security/etrade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bonds
- Brokerage
- Financial
- Futures
- Options
- Stocks
- Trading
---
