---
api_specs:
- filename: pulsoid-features-api-openapi.yml
  format: yaml
  label: Pulsoid Features API
  slug: pulsoid-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-features-api-openapi.yml
- filename: pulsoid-geometry-dash-api-openapi.yml
  format: yaml
  label: Pulsoid Geometry Dash API
  slug: pulsoid-geometry-dash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-geometry-dash-api-openapi.yml
- filename: pulsoid-heart-rate-api-openapi.yml
  format: yaml
  label: Pulsoid Heart Rate API
  slug: pulsoid-heart-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-heart-rate-api-openapi.yml
- filename: pulsoid-oauth2-api-openapi.yml
  format: yaml
  label: Pulsoid OAuth2 API
  slug: pulsoid-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-oauth2-api-openapi.yml
- filename: pulsoid-profile-api-openapi.yml
  format: yaml
  label: Pulsoid Profile API
  slug: pulsoid-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-profile-api-openapi.yml
- filename: pulsoid-statistics-api-openapi.yml
  format: yaml
  label: Pulsoid Statistics API
  slug: pulsoid-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-statistics-api-openapi.yml
- filename: pulsoid-token-api-openapi.yml
  format: yaml
  label: Pulsoid Token API
  slug: pulsoid-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-token-api-openapi.yml
- filename: pulsoid-widgets-api-openapi.yml
  format: yaml
  label: Pulsoid Widgets API
  slug: pulsoid-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/openapi/pulsoid-widgets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pulsoid.net
  spf: false
hosts:
- cert_expires: Sep 16 04:38:57 2026 GMT
  host: pulsoid.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 17:29:23 2026 GMT
  host: docs.pulsoid.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 20:58:57 2026 GMT
  host: dev.pulsoid.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pulsoid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulsoid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Pulsoid
provider_slug: pulsoid
slug: pulsoid-domain-security
source_filename: pulsoid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pulsoid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:38:57 2026 GMT\n  hsts: false\n- host: docs.pulsoid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 17:29:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.pulsoid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:58:57 2026 GMT\n  hsts: false\ndomains:\n- domain: pulsoid.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulsoid/refs/heads/main/security/pulsoid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Heart Rate
- Health
- Wearables
- Real-Time
- Streaming
- WebSocket
- OAuth2
---
