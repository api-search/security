---
api_specs:
- filename: bitoasis-exchange-openapi.yml
  format: yaml
  label: BitOasis Exchange API
  slug: bitoasis-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitoasis/refs/heads/main/openapi/bitoasis-exchange-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bitoasis.net
  spf: true
hosts:
- cert_expires: Oct  2 12:27:29 2026 GMT
  host: bitoasis.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 14:16:21 2026 GMT
  host: api.bitoasis.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitoasis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitOasis, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BitOasis
provider_slug: bitoasis
slug: bitoasis-domain-security
source_filename: bitoasis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitoasis.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:27:29 2026 GMT\n  hsts: null\n- host: api.bitoasis.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:16:21 2026 GMT\n  hsts: null\ndomains:\n- domain: bitoasis.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitoasis/refs/heads/main/security/bitoasis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- Cryptocurrency
- Exchange
- Trading
- Digital Assets
- Bitcoin
- MENA
- Fintech
- MCP
---
