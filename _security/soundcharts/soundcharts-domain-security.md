---
api_specs:
- filename: soundcharts-album-api-openapi.yml
  format: yaml
  label: Soundcharts Album API
  slug: soundcharts-album-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-album-api-openapi.yml
- filename: soundcharts-artist-api-openapi.yml
  format: yaml
  label: Soundcharts Artist API
  slug: soundcharts-artist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-artist-api-openapi.yml
- filename: soundcharts-chart-api-openapi.yml
  format: yaml
  label: Soundcharts Chart API
  slug: soundcharts-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-chart-api-openapi.yml
- filename: soundcharts-metrics-api-openapi.yml
  format: yaml
  label: Soundcharts Metrics API
  slug: soundcharts-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-metrics-api-openapi.yml
- filename: soundcharts-playlist-api-openapi.yml
  format: yaml
  label: Soundcharts Playlist API
  slug: soundcharts-playlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-playlist-api-openapi.yml
- filename: soundcharts-radio-api-openapi.yml
  format: yaml
  label: Soundcharts Radio API
  slug: soundcharts-radio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-radio-api-openapi.yml
- filename: soundcharts-referential-api-openapi.yml
  format: yaml
  label: Soundcharts Referential API
  slug: soundcharts-referential-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-referential-api-openapi.yml
- filename: soundcharts-search-api-openapi.yml
  format: yaml
  label: Soundcharts Search API
  slug: soundcharts-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-search-api-openapi.yml
- filename: soundcharts-song-api-openapi.yml
  format: yaml
  label: Soundcharts Song API
  slug: soundcharts-song-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcharts/refs/heads/main/openapi/soundcharts-song-api-openapi.yml
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
