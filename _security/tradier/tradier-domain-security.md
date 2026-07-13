---
api_specs:
- filename: tradier-openapi.yml
  format: yaml
  label: Tradier Brokerage API
  slug: brokerage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/openapi/tradier-openapi.yml
- filename: tradier-asyncapi.yml
  format: yaml
  label: Tradier Streaming API
  slug: streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/asyncapi/tradier-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tradier.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: tradier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 22:58:42 2026 GMT
  host: docs.tradier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: api.tradier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tradier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tradier, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tradier
provider_slug: tradier
slug: tradier-domain-security
source_filename: tradier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tradier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tradier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:58:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tradier.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tradier.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradier/refs/heads/main/security/tradier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Trading
- Stocks
- Options
- Brokerage
- Streaming
---
