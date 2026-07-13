---
api_specs:
- filename: coindcx-asyncapi.yml
  format: yaml
  label: CoinDCX Streaming Socket.IO API
  slug: streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/coindcx/refs/heads/main/asyncapi/coindcx-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: coindcx.com
  spf: true
hosts:
- cert_expires: Sep  6 20:30:25 2026 GMT
  host: docs.coindcx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: stream.coindcx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Coindcx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoinDCX, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CoinDCX
provider_slug: coindcx
slug: coindcx-domain-security
source_filename: coindcx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.coindcx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 20:30:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: stream.coindcx.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coindcx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coindcx/refs/heads/main/security/coindcx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- Public APIs
---
