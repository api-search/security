---
api_specs:
- filename: radar-io-addresses-api-openapi.yml
  format: yaml
  label: Radar Addresses API
  slug: radar-io-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-addresses-api-openapi.yml
- filename: radar-io-events-api-openapi.yml
  format: yaml
  label: Radar Events API
  slug: radar-io-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-events-api-openapi.yml
- filename: radar-io-geocoding-api-openapi.yml
  format: yaml
  label: Radar Geocoding API
  slug: radar-io-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-geocoding-api-openapi.yml
- filename: radar-io-geofences-api-openapi.yml
  format: yaml
  label: Radar Geofences API
  slug: radar-io-geofences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-geofences-api-openapi.yml
- filename: radar-io-routing-api-openapi.yml
  format: yaml
  label: Radar Routing API
  slug: radar-io-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-routing-api-openapi.yml
- filename: radar-io-search-api-openapi.yml
  format: yaml
  label: Radar Search API
  slug: radar-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-search-api-openapi.yml
- filename: radar-io-tiles-api-openapi.yml
  format: yaml
  label: Radar Tiles API
  slug: radar-io-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-tiles-api-openapi.yml
- filename: radar-io-track-api-openapi.yml
  format: yaml
  label: Radar Track API
  slug: radar-io-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-track-api-openapi.yml
- filename: radar-io-trips-api-openapi.yml
  format: yaml
  label: Radar Trips API
  slug: radar-io-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-trips-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: radar.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: radar.io
  spf: true
hosts:
- cert_expires: Aug 25 05:23:12 2026 GMT
  host: radar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 09:21:30 2026 GMT
  host: api.radar.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Radar Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Radar, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Radar
provider_slug: radar-io
slug: radar-io-domain-security
source_filename: radar-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: radar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 05:23:12 2026 GMT\n  hsts: false\n- host: api.radar.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 09:21:30 2026 GMT\n  hsts: null\ndomains:\n- domain: radar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: radar.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/security/radar-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Location
- Geocoding
- Geofencing
- Maps
- Routing
---
