---
api_specs:
- filename: cargoson-openapi.yml
  format: yaml
  label: Cargoson Shipments API
  slug: shipments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/openapi/cargoson-openapi.yml
- filename: cargoson-openapi.yml
  format: yaml
  label: Cargoson Price Requests & Quotes API
  slug: price-requests-quotes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/openapi/cargoson-openapi.yml
- filename: cargoson-openapi.yml
  format: yaml
  label: Cargoson Transports & Tracking API
  slug: transports-tracking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/openapi/cargoson-openapi.yml
- filename: cargoson-openapi.yml
  format: yaml
  label: Cargoson Carriers & Services API
  slug: carriers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/openapi/cargoson-openapi.yml
- filename: cargoson-openapi.yml
  format: yaml
  label: Cargoson Addresses API
  slug: addresses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/openapi/cargoson-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cargoson.com
  spf: true
hosts:
- cert_expires: Sep 16 13:42:34 2026 GMT
  host: www.cargoson.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cargoson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cargoson, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cargoson
provider_slug: cargoson
slug: cargoson-domain-security
source_filename: cargoson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cargoson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 13:42:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cargoson.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargoson/refs/heads/main/security/cargoson-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Transport Management
- TMS
- Freight
- Shipping
- Logistics
- Carriers
---
