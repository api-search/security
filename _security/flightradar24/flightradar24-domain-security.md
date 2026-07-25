---
api_specs:
- filename: flightradar24-airlines-api-openapi.yml
  format: yaml
  label: Flightradar24 Airlines API
  slug: flightradar24-airlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-airlines-api-openapi.yml
- filename: flightradar24-airports-api-openapi.yml
  format: yaml
  label: Flightradar24 Airports API
  slug: flightradar24-airports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-airports-api-openapi.yml
- filename: flightradar24-flight-summary-api-openapi.yml
  format: yaml
  label: Flightradar24 Flight Summary API
  slug: flightradar24-flight-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-flight-summary-api-openapi.yml
- filename: flightradar24-flight-tracks-api-openapi.yml
  format: yaml
  label: Flightradar24 Flight Tracks API
  slug: flightradar24-flight-tracks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-flight-tracks-api-openapi.yml
- filename: flightradar24-historic-events-api-openapi.yml
  format: yaml
  label: Flightradar24 Historic Events API
  slug: flightradar24-historic-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-historic-events-api-openapi.yml
- filename: flightradar24-historic-positions-api-openapi.yml
  format: yaml
  label: Flightradar24 Historic Positions API
  slug: flightradar24-historic-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-historic-positions-api-openapi.yml
- filename: flightradar24-live-positions-api-openapi.yml
  format: yaml
  label: Flightradar24 Live Positions API
  slug: flightradar24-live-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-live-positions-api-openapi.yml
- filename: flightradar24-usage-api-openapi.yml
  format: yaml
  label: Flightradar24 Usage API
  slug: flightradar24-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/openapi/flightradar24-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flightradar24.com
  spf: true
hosts:
- cert_expires: Aug 19 17:57:32 2026 GMT
  host: fr24api.flightradar24.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flightradar24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flightradar24, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flightradar24
provider_slug: flightradar24
slug: flightradar24-domain-security
source_filename: flightradar24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fr24api.flightradar24.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 17:57:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flightradar24.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightradar24/refs/heads/main/security/flightradar24-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Aviation
- Flight Tracking
- Real-Time
- Aircraft
- Airports
- Airlines
- ADS-B
- Historical Data
---
