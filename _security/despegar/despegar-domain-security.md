---
api_specs:
- filename: despegar-hotels-openapi.json
  format: json
  label: Despegar Hotels API
  slug: despegar-hotels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-hotels-openapi.json
- filename: despegar-flights-openapi.json
  format: json
  label: Despegar Flights API
  slug: despegar-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-flights-openapi.json
- filename: despegar-activities-openapi.json
  format: json
  label: Despegar Activities API
  slug: despegar-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-activities-openapi.json
- filename: despegar-booking-openapi.json
  format: json
  label: Despegar Booking API
  slug: despegar-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-booking-openapi.json
- filename: despegar-aftersales-openapi.json
  format: json
  label: Despegar Aftersales API
  slug: despegar-aftersales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-aftersales-openapi.json
- filename: despegar-geo-openapi.json
  format: json
  label: Despegar Common Assets API
  slug: despegar-common-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/openapi/despegar-geo-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: despegar.com
  spf: true
hosts:
- cert_expires: Sep  1 23:59:59 2026 GMT
  host: www.despegar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Despegar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Despegar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Despegar
provider_slug: despegar
slug: despegar-domain-security
source_filename: despegar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.despegar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: despegar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/despegar/refs/heads/main/security/despegar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Travel
- Hotels
- Flights
- Booking
- Tourism
- Latin America
- B2B
- MCP
---
