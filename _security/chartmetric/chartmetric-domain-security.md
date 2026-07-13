---
api_specs:
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Artists API
  slug: artists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Tracks API
  slug: tracks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Albums API
  slug: albums
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Playlists API
  slug: playlists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Charts API
  slug: charts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Stats and Metrics API
  slug: stats-metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
- filename: chartmetric-openapi.yml
  format: yaml
  label: Chartmetric Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/openapi/chartmetric-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chartmetric.com
  spf: true
hosts:
- cert_expires: Oct  5 21:43:16 2026 GMT
  host: www.chartmetric.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 15:59:42 2026 GMT
  host: apidocs.chartmetric.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: api.chartmetric.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chartmetric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chartmetric, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chartmetric
provider_slug: chartmetric
slug: chartmetric-domain-security
source_filename: chartmetric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chartmetric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:43:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apidocs.chartmetric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:59:42 2026 GMT\n  hsts: false\n- host: api.chartmetric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: chartmetric.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chartmetric/refs/heads/main/security/chartmetric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Analytics
- Artist Intelligence
- Streaming
- Charts
---
