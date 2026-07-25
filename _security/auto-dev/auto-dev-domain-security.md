---
api_specs:
- filename: auto-dev-dealers-api-openapi.yml
  format: yaml
  label: Auto.dev Dealers API
  slug: auto-dev-dealers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-dealers-api-openapi.yml
- filename: auto-dev-listings-api-openapi.yml
  format: yaml
  label: Auto.dev Listings API
  slug: auto-dev-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-listings-api-openapi.yml
- filename: auto-dev-market-value-api-openapi.yml
  format: yaml
  label: Auto.dev Market Value API
  slug: auto-dev-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-market-value-api-openapi.yml
- filename: auto-dev-recalls-api-openapi.yml
  format: yaml
  label: Auto.dev Recalls API
  slug: auto-dev-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-recalls-api-openapi.yml
- filename: auto-dev-vin-decoding-api-openapi.yml
  format: yaml
  label: Auto.dev VIN Decoding API
  slug: auto-dev-vin-decoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-vin-decoding-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: auto.dev
  spf: true
hosts:
- cert_expires: Aug 28 08:31:34 2026 GMT
  host: www.auto.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 08:31:34 2026 GMT
  host: docs.auto.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 08:31:34 2026 GMT
  host: api.auto.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Auto Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Auto.dev, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Auto.dev
provider_slug: auto-dev
slug: auto-dev-domain-security
source_filename: auto-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.auto.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:31:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.auto.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:31:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.auto.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:31:34 2026 GMT\n  hsts: false\ndomains:\n- domain: auto.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/security/auto-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Vehicle Data
- VIN Decoding
- Vehicle Listings
- Recalls
---
