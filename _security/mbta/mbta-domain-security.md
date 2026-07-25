---
api_specs:
- filename: mbta-alerts-api-openapi.yml
  format: yaml
  label: MBTA Alerts API
  slug: mbta-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-alerts-api-openapi.yml
- filename: mbta-facilities-api-openapi.yml
  format: yaml
  label: MBTA Facilities API
  slug: mbta-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-facilities-api-openapi.yml
- filename: mbta-lines-api-openapi.yml
  format: yaml
  label: MBTA Lines API
  slug: mbta-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-lines-api-openapi.yml
- filename: mbta-predictions-api-openapi.yml
  format: yaml
  label: MBTA Predictions API
  slug: mbta-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-predictions-api-openapi.yml
- filename: mbta-routepatterns-api-openapi.yml
  format: yaml
  label: MBTA RoutePatterns API
  slug: mbta-routepatterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-routepatterns-api-openapi.yml
- filename: mbta-routes-api-openapi.yml
  format: yaml
  label: MBTA Routes API
  slug: mbta-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-routes-api-openapi.yml
- filename: mbta-schedules-api-openapi.yml
  format: yaml
  label: MBTA Schedules API
  slug: mbta-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-schedules-api-openapi.yml
- filename: mbta-services-api-openapi.yml
  format: yaml
  label: MBTA Services API
  slug: mbta-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-services-api-openapi.yml
- filename: mbta-shapes-api-openapi.yml
  format: yaml
  label: MBTA Shapes API
  slug: mbta-shapes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-shapes-api-openapi.yml
- filename: mbta-stops-api-openapi.yml
  format: yaml
  label: MBTA Stops API
  slug: mbta-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-stops-api-openapi.yml
- filename: mbta-trips-api-openapi.yml
  format: yaml
  label: MBTA Trips API
  slug: mbta-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-trips-api-openapi.yml
- filename: mbta-vehicles-api-openapi.yml
  format: yaml
  label: MBTA Vehicles API
  slug: mbta-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/openapi/mbta-vehicles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mbta.com
  spf: true
hosts:
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: www.mbta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: api-v3.mbta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mbta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MBTA, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MBTA
provider_slug: mbta
slug: mbta-domain-security
source_filename: mbta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mbta.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-v3.mbta.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mbta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mbta/refs/heads/main/security/mbta-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Boston
- Massachusetts
- Public Transportation
- Real-Time
- Transit
---
