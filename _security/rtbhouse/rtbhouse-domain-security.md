---
api_specs:
- filename: rtbhouse-advertisers-api-openapi.yml
  format: yaml
  label: RTB House Advertisers API
  slug: rtbhouse-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/openapi/rtbhouse-advertisers-api-openapi.yml
- filename: rtbhouse-dev-api-openapi.yml
  format: yaml
  label: RTB House Dev API
  slug: rtbhouse-dev-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/openapi/rtbhouse-dev-api-openapi.yml
- filename: rtbhouse-statistics-api-openapi.yml
  format: yaml
  label: RTB House Statistics API
  slug: rtbhouse-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/openapi/rtbhouse-statistics-api-openapi.yml
- filename: rtbhouse-tokens-api-openapi.yml
  format: yaml
  label: RTB House Tokens API
  slug: rtbhouse-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/openapi/rtbhouse-tokens-api-openapi.yml
- filename: rtbhouse-user-api-openapi.yml
  format: yaml
  label: RTB House User API
  slug: rtbhouse-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/openapi/rtbhouse-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rtbhouse.com
  spf: true
hosts:
- cert_expires: Sep 26 19:45:38 2026 GMT
  host: www.rtbhouse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 09:31:34 2026 GMT
  host: api.panel.rtbhouse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: 'HSTS confirmed by direct probe on 2026-08-13 — HEAD https://api.panel.rtbhouse.com/v5/healthcheck returned 200 with strict-transport-security: max-age=31536000 (the automated probe recorded null because the host root returns an nginx 404).'
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rtbhouse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RTB House, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RTB House
provider_slug: rtbhouse
slug: rtbhouse-domain-security
source_filename: rtbhouse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rtbhouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:45:38 2026 GMT\n  hsts: false\n- host: api.panel.rtbhouse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 09:31:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: 'HSTS confirmed by direct probe on 2026-08-13 — HEAD https://api.panel.rtbhouse.com/v5/healthcheck\n    returned 200 with strict-transport-security: max-age=31536000 (the automated probe\n    recorded null because the host root returns an nginx 404).'\ndomains:\n- domain: rtbhouse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rtbhouse/refs/heads/main/security/rtbhouse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Retargeting
- Programmatic
- DSP
- Deep Learning
- RTB
- Performance Marketing
---
