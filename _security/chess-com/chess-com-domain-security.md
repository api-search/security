---
api_specs:
- filename: chess-com-published-data-api-openapi.yml
  format: yaml
  label: Chess.com Published Data API
  slug: chess-com-published-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chess-com/refs/heads/main/openapi/chess-com-published-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chess.com
  spf: true
hosts:
- cert_expires: Aug 16 23:45:12 2026 GMT
  host: www.chess.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 23:45:12 2026 GMT
  host: api.chess.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chess Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chess.com, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chess.com
provider_slug: chess-com
slug: chess-com-domain-security
source_filename: chess-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chess.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:45:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.chess.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:45:12 2026 GMT\n  hsts: null\ndomains:\n- domain: chess.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chess-com/refs/heads/main/security/chess-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chess
- Gaming
- Online Games
- Sports
- Community
- Education
---
