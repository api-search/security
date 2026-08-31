---
api_specs:
- filename: transit-alerts-api-openapi.yml
  format: yaml
  label: Transit Alerts API
  slug: transit-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-alerts-api-openapi.yml
- filename: transit-departures-api-openapi.yml
  format: yaml
  label: Transit Departures API
  slug: transit-departures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-departures-api-openapi.yml
- filename: transit-mobility-api-openapi.yml
  format: yaml
  label: Transit Mobility API
  slug: transit-mobility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-mobility-api-openapi.yml
- filename: transit-networks-api-openapi.yml
  format: yaml
  label: Transit Networks API
  slug: transit-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-networks-api-openapi.yml
- filename: transit-routes-api-openapi.yml
  format: yaml
  label: Transit Routes API
  slug: transit-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-routes-api-openapi.yml
- filename: transit-stops-api-openapi.yml
  format: yaml
  label: Transit Stops API
  slug: transit-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-stops-api-openapi.yml
- filename: transit-trips-api-openapi.yml
  format: yaml
  label: Transit Trips API
  slug: transit-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/openapi/transit-trips-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: transitapp.com
  spf: true
hosts:
- cert_expires: Aug 18 01:29:20 2026 GMT
  host: transitapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 11:34:48 2026 GMT
  host: api-doc.transitapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transit, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transit
provider_slug: transit
slug: transit-domain-security
source_filename: transit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transitapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 01:29:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-doc.transitapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 11:34:48 2026 GMT\n  hsts: false\ndomains:\n- domain: transitapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transit/refs/heads/main/security/transit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Public Transit
- Real-Time
- Trip Planning
- Multimodal
- GTFS
- GOFS
- Mobility
- Shared Mobility
---
