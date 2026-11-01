---
api_specs:
- filename: chartmetric-charts-api-openapi.yml
  format: yaml
  label: Chartmetric Charts API
  slug: chartmetric-charts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-charts-api-openapi.yml
- filename: chartmetric-search-api-openapi.yml
  format: yaml
  label: Chartmetric Search API
  slug: chartmetric-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-search-api-openapi.yml
- filename: chartmetric-album-api-openapi.yml
  format: yaml
  label: Chartmetric Album API
  slug: chartmetric-album-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-album-api-openapi.yml
- filename: chartmetric-artist-api-openapi.yml
  format: yaml
  label: Chartmetric Artist API
  slug: chartmetric-artist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-artist-api-openapi.yml
- filename: chartmetric-brand-api-openapi.yml
  format: yaml
  label: Chartmetric Brand API
  slug: chartmetric-brand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-brand-api-openapi.yml
- filename: chartmetric-city-api-openapi.yml
  format: yaml
  label: Chartmetric City API
  slug: chartmetric-city-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-city-api-openapi.yml
- filename: chartmetric-country-api-openapi.yml
  format: yaml
  label: Chartmetric Country API
  slug: chartmetric-country-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-country-api-openapi.yml
- filename: chartmetric-curator-api-openapi.yml
  format: yaml
  label: Chartmetric Curator API
  slug: chartmetric-curator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-curator-api-openapi.yml
- filename: chartmetric-event-api-openapi.yml
  format: yaml
  label: Chartmetric Event API
  slug: chartmetric-event-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-event-api-openapi.yml
- filename: chartmetric-festival-api-openapi.yml
  format: yaml
  label: Chartmetric Festival API
  slug: chartmetric-festival-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-festival-api-openapi.yml
- filename: chartmetric-genre-api-openapi.yml
  format: yaml
  label: Chartmetric Genre API
  slug: chartmetric-genre-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-genre-api-openapi.yml
- filename: chartmetric-playlist-api-openapi.yml
  format: yaml
  label: Chartmetric Playlist API
  slug: chartmetric-playlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-playlist-api-openapi.yml
- filename: chartmetric-radio-api-openapi.yml
  format: yaml
  label: Chartmetric Radio API
  slug: chartmetric-radio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-radio-api-openapi.yml
- filename: chartmetric-sns-api-openapi.yml
  format: yaml
  label: Chartmetric SNS API
  slug: chartmetric-sns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-sns-api-openapi.yml
- filename: chartmetric-token-api-openapi.yml
  format: yaml
  label: Chartmetric Token API
  slug: chartmetric-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-token-api-openapi.yml
- filename: chartmetric-track-api-openapi.yml
  format: yaml
  label: Chartmetric Track API
  slug: chartmetric-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-track-api-openapi.yml
- filename: chartmetric-venue-api-openapi.yml
  format: yaml
  label: Chartmetric Venue API
  slug: chartmetric-venue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartmetric/openapi/chartmetric-venue-api-openapi.yml
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
hosts_probed: 3
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
source_yaml_url: https://artifacts.apis.io/chartmetric/security/chartmetric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Analytics
- Artist Intelligence
- Streaming
- Charts
---
