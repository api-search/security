---
api_specs:
- filename: bitfinex-asyncapi.yml
  format: yaml
  label: Bitfinex
  slug: bitfinex
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitfinex/refs/heads/main/asyncapi/bitfinex-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bitfinex.com
  spf: true
hosts:
- cert_expires: Oct  2 14:16:38 2026 GMT
  host: docs.bitfinex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitfinex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitfinex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bitfinex
provider_slug: bitfinex
slug: bitfinex-domain-security
source_filename: bitfinex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.bitfinex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:16:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bitfinex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitfinex/refs/heads/main/security/bitfinex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Public APIs
---
