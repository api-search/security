---
api_specs:
- filename: flightlabs-aircraft-api-openapi.yml
  format: yaml
  label: FlightLabs Aircraft API
  slug: flightlabs-aircraft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightlabs/refs/heads/main/openapi/flightlabs-aircraft-api-openapi.yml
- filename: flightlabs-airlines-api-openapi.yml
  format: yaml
  label: FlightLabs Airlines API
  slug: flightlabs-airlines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightlabs/refs/heads/main/openapi/flightlabs-airlines-api-openapi.yml
- filename: flightlabs-airports-api-openapi.yml
  format: yaml
  label: FlightLabs Airports API
  slug: flightlabs-airports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightlabs/refs/heads/main/openapi/flightlabs-airports-api-openapi.yml
- filename: flightlabs-flights-api-openapi.yml
  format: yaml
  label: FlightLabs Flights API
  slug: flightlabs-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightlabs/refs/heads/main/openapi/flightlabs-flights-api-openapi.yml
- filename: flightlabs-geography-api-openapi.yml
  format: yaml
  label: FlightLabs Geography API
  slug: flightlabs-geography-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightlabs/refs/heads/main/openapi/flightlabs-geography-api-openapi.yml
- filename: flightlabs-pricing-api-openapi.yml
  format: yaml
  label: FlightLabs Pricing API
  slug: flightlabs-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightlabs/refs/heads/main/openapi/flightlabs-pricing-api-openapi.yml
- filename: flightlabs-routes-api-openapi.yml
  format: yaml
  label: FlightLabs Routes API
  slug: flightlabs-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightlabs/refs/heads/main/openapi/flightlabs-routes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goflightlabs.com
  spf: true
hosts:
- cert_expires: Aug 14 19:56:04 2026 GMT
  host: www.goflightlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 19:56:04 2026 GMT
  host: app.goflightlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flightlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlightLabs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FlightLabs
provider_slug: flightlabs
slug: flightlabs-domain-security
source_filename: flightlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goflightlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 19:56:04 2026 GMT\n  hsts: false\n- host: app.goflightlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 19:56:04 2026 GMT\n  hsts: false\ndomains:\n- domain: goflightlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightlabs/refs/heads/main/security/flightlabs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aviation
- Flights
- Airlines
- Airports
- Flight Tracking
- Travel
- Real-Time Data
---
