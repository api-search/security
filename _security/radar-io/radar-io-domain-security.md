---
api_specs:
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Geocoding API
  slug: radar-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Search & Autocomplete API
  slug: radar-search-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Routing, Distance & Matrix API
  slug: radar-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Geofences API
  slug: radar-geofences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Track & Users API
  slug: radar-track-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Events API
  slug: radar-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Trips API
  slug: radar-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Address Verification API
  slug: radar-address-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
- filename: radar-io-openapi.yml
  format: yaml
  label: Radar Maps & Tiles API
  slug: radar-maps-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radar-io/refs/heads/main/openapi/radar-io-openapi.yml
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
