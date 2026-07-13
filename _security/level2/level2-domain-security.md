---
api_specs:
- filename: level2-strategy-builder-openapi.yml
  format: yaml
  label: Level2 Strategy Builder API
  slug: strategy-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-strategy-builder-openapi.yml
- filename: level2-tradestation-integration-openapi.yml
  format: yaml
  label: Level2 TradeStation Integration API
  slug: tradestation-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/openapi/level2-tradestation-integration-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trylevel2.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bytemine.io
  spf: true
hosts:
- cert_expires: Sep 13 08:58:44 2026 GMT
  host: www.trylevel2.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:15:15 2026 GMT
  host: learn.trylevel2.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: app.bytemine.io
  https: false
kind: domain-security
layout: security
method: probed
name: Level2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for level2, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: level2
provider_slug: level2
slug: level2-domain-security
source_filename: level2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trylevel2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:58:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: learn.trylevel2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:15:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.bytemine.io\n  https: false\ndomains:\n- domain: trylevel2.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bytemine.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/level2/refs/heads/main/security/level2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
