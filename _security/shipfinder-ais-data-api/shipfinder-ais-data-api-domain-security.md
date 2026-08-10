---
api_specs:
- filename: shipfinder-ais-data-api-ais-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API AIS Dataset API
  slug: shipfinder-ais-data-api-ais-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-ais-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-china-coastline-warning-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API China Coastline Warning Dataset API
  slug: shipfinder-ais-data-api-china-coastline-warning-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-china-coastline-warning-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-event-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Event Dataset API
  slug: shipfinder-ais-data-api-event-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-event-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-history-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API History Dataset API
  slug: shipfinder-ais-data-api-history-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-history-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-meteorology-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Meteorology Dataset API
  slug: shipfinder-ais-data-api-meteorology-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-meteorology-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-prediction-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Prediction Dataset API
  slug: shipfinder-ais-data-api-prediction-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-prediction-dataset-api-openapi.yml
- filename: shipfinder-ais-data-api-voyage-dataset-api-openapi.yml
  format: yaml
  label: ShipFinder AIS Data API Voyage Dataset API
  slug: shipfinder-ais-data-api-voyage-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/openapi/shipfinder-ais-data-api-voyage-dataset-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shipfinder.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: elaneglobal.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: www.shipfinder.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 09:01:36 2026 GMT
  host: api.elaneglobal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shipfinder Ais Data Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShipFinder AIS Data API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ShipFinder AIS Data API
provider_slug: shipfinder-ais-data-api
slug: shipfinder-ais-data-api-domain-security
source_filename: shipfinder-ais-data-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.shipfinder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: false\n- host: api.elaneglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 09:01:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: shipfinder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: elaneglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shipfinder-ais-data-api/refs/heads/main/security/shipfinder-ais-data-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIS
- Maritime Data
- Vessel Tracking
- Ship Tracking
- Vessel Data
- Historical AIS
- Geospatial
- GIS
- Logistics
- Supply Chain
- Weather
- Meteorology
- Trade
- Commodities
- Compliance
- Risk
- Event Streaming
- Webhooks
---
