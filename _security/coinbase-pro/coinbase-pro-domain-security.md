---
api_specs:
- filename: coinbase-pro-asyncapi.yml
  format: yaml
  label: Coinbase Pro
  slug: coinbase-pro
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinbase-pro/refs/heads/main/asyncapi/coinbase-pro-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@coinbase.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coinbase.com
  spf: true
hosts:
- cert_expires: Sep  8 09:13:32 2026 GMT
  host: docs.pro.coinbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinbase Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinbase Pro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coinbase Pro
provider_slug: coinbase-pro
slug: coinbase-pro-domain-security
source_filename: coinbase-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.pro.coinbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:13:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coinbase.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@coinbase.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinbase-pro/refs/heads/main/security/coinbase-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Public APIs
---
