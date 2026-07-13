---
api_specs:
- filename: spx-graphics-control-api-openapi.yml
  format: yaml
  label: SPX Graphics Control API
  slug: spx-graphics-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spx/refs/heads/main/openapi/spx-graphics-control-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: spxgraphics.com
  spf: false
hosts:
- cert_expires: Aug 18 12:11:14 2026 GMT
  host: spxgraphics.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPX Graphics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: SPX Graphics
provider_slug: spx
slug: spx-domain-security
source_filename: spx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spxgraphics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 12:11:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: spxgraphics.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spx/refs/heads/main/security/spx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Broadcast
- Graphics
- Live Production
- Media
- Streaming
- Video Production
- Fortune 1000
---
