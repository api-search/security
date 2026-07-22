---
api_specs:
- filename: sanas-stream-asyncapi.yml
  format: yaml
  label: Sanas Stream API
  slug: sanas-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanas/refs/heads/main/asyncapi/sanas-stream-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sanas.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sanaslt.com
  spf: false
hosts:
- cert_expires: Sep 23 22:06:46 2026 GMT
  host: sanas.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:02:40 2026 GMT
  host: developer.sanas.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.sanaslt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sanas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sanas, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sanas
provider_slug: sanas
slug: sanas-domain-security
source_filename: sanas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sanas.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:06:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.sanas.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:02:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sanaslt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sanas.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sanaslt.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanas/refs/heads/main/security/sanas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Speech AI
- Voice AI
- Accent Translation
- Language Translation
- Speech Enhancement
- Real-Time Audio
- SDK
- WebSocket
- Contact Center
---
