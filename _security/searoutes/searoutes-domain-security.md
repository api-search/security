---
api_specs:
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Ocean Routing API
  slug: searoutes-ocean-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Geocoding API
  slug: searoutes-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes CO2 Emissions API
  slug: searoutes-co2-emissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Vessel Tracking API
  slug: searoutes-vessel-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Search & Carriers API
  slug: searoutes-search-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
- filename: searoutes-openapi.yml
  format: yaml
  label: Searoutes Weather API
  slug: searoutes-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/openapi/searoutes-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: searoutes.com
  spf: true
hosts:
- cert_expires: Sep 17 02:35:51 2026 GMT
  host: searoutes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 00:03:31 2026 GMT
  host: developer.searoutes.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: api.searoutes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Searoutes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Searoutes, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Searoutes
provider_slug: searoutes
slug: searoutes-domain-security
source_filename: searoutes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: searoutes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 02:35:51 2026 GMT\n  hsts: false\n- host: developer.searoutes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 00:03:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.searoutes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: searoutes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searoutes/refs/heads/main/security/searoutes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Maritime
- Sea Routing
- Ocean Freight
- CO2 Emissions
- Carbon Accounting
- Vessel Tracking
- AIS
- Geocoding
- Logistics
- Supply Chain
---
