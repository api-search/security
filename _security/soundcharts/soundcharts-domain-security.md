---
api_specs:
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Artists API
  slug: artists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Songs API
  slug: songs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Albums API
  slug: albums
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Playlists API
  slug: playlists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Charts API
  slug: charts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Streaming and Social Metrics API
  slug: streaming-social-metrics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
- filename: soundcharts-openapi.yml
  format: yaml
  label: Soundcharts Radio API
  slug: radio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soundcharts.com
  spf: true
hosts:
- cert_expires: Sep 22 01:02:39 2026 GMT
  host: soundcharts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 01:02:38 2026 GMT
  host: developers.soundcharts.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 20:52:39 2026 GMT
  host: customer.api.soundcharts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soundcharts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soundcharts, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Soundcharts
provider_slug: soundcharts
slug: soundcharts-domain-security
source_filename: soundcharts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soundcharts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:02:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.soundcharts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:02:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: customer.api.soundcharts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:52:39 2026 GMT\n  hsts: null\ndomains:\n- domain: soundcharts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/security/soundcharts-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Analytics
- Market Intelligence
- Metadata
- Streaming
- Charts
---
