---
api_specs:
- filename: transitland-agencies-api-openapi.yml
  format: yaml
  label: TransitLand Agencies API
  slug: transitland-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-agencies-api-openapi.yml
- filename: transitland-feed-versions-api-openapi.yml
  format: yaml
  label: TransitLand Feed Versions API
  slug: transitland-feed-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-feed-versions-api-openapi.yml
- filename: transitland-feeds-api-openapi.yml
  format: yaml
  label: TransitLand Feeds API
  slug: transitland-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-feeds-api-openapi.yml
- filename: transitland-onestop-id-api-openapi.yml
  format: yaml
  label: TransitLand Onestop Id API
  slug: transitland-onestop-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-onestop-id-api-openapi.yml
- filename: transitland-operators-api-openapi.yml
  format: yaml
  label: TransitLand Operators API
  slug: transitland-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-operators-api-openapi.yml
- filename: transitland-routes-api-openapi.yml
  format: yaml
  label: TransitLand Routes API
  slug: transitland-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-routes-api-openapi.yml
- filename: transitland-stops-api-openapi.yml
  format: yaml
  label: TransitLand Stops API
  slug: transitland-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-stops-api-openapi.yml
- filename: transitland-street-routing-api-openapi.yml
  format: yaml
  label: TransitLand Street routing API
  slug: transitland-street-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-street-routing-api-openapi.yml
- filename: transitland-transit-routing-api-openapi.yml
  format: yaml
  label: TransitLand Transit routing API
  slug: transitland-transit-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-transit-routing-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: transit.land
  spf: true
hosts:
- cert_expires: Jan  8 14:04:29 2027 GMT
  host: www.transit.land
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Transitland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TransitLand, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TransitLand
provider_slug: transitland
slug: transitland-domain-security
source_filename: transitland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transit.land\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 14:04:29 2027 GMT\n  hsts: false\ndomains:\n- domain: transit.land\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/security/transitland-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Public APIs
- Transit
- GTFS
- Open Data
- Routing
- Geospatial
---
