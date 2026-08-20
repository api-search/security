---
api_specs:
- filename: moovit-general-api-openapi.yml
  format: yaml
  label: Moovit General API
  slug: moovit-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/openapi/moovit-general-api-openapi.yml
- filename: moovit-gtfsrealtime-api-openapi.yml
  format: yaml
  label: Moovit GTFSRealtime API
  slug: moovit-gtfsrealtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/openapi/moovit-gtfsrealtime-api-openapi.yml
- filename: moovit-lines-api-openapi.yml
  format: yaml
  label: Moovit Lines API
  slug: moovit-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/openapi/moovit-lines-api-openapi.yml
- filename: moovit-nearby-api-openapi.yml
  format: yaml
  label: Moovit Nearby API
  slug: moovit-nearby-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/openapi/moovit-nearby-api-openapi.yml
- filename: moovit-realtime-api-openapi.yml
  format: yaml
  label: Moovit RealTime API
  slug: moovit-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/openapi/moovit-realtime-api-openapi.yml
- filename: moovit-search-api-openapi.yml
  format: yaml
  label: Moovit Search API
  slug: moovit-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/openapi/moovit-search-api-openapi.yml
- filename: moovit-servicealerts-api-openapi.yml
  format: yaml
  label: Moovit ServiceAlerts API
  slug: moovit-servicealerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/openapi/moovit-servicealerts-api-openapi.yml
- filename: moovit-stops-api-openapi.yml
  format: yaml
  label: Moovit Stops API
  slug: moovit-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/openapi/moovit-stops-api-openapi.yml
- filename: moovit-tripplan-api-openapi.yml
  format: yaml
  label: Moovit TripPlan API
  slug: moovit-tripplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/openapi/moovit-tripplan-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moovit.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moovitapp.com
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: moovit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api-docs.moovit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: app5.moovitapp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moovit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moovit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moovit
provider_slug: moovit
slug: moovit-domain-security
source_filename: moovit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moovit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-docs.moovit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: false\n- host: app5.moovitapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moovit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: moovitapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moovit/refs/heads/main/security/moovit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transit
- Public Transit
- Mobility
- Mobility As A Service
- MaaS
- Trip Planning
- Multimodal Routing
- Real-Time
- GTFS
- GTFS Realtime
- Service Alerts
- Smart Cities
- Transportation
- Mobileye
- Intel
---
