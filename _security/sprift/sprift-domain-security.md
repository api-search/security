---
api_specs:
- filename: sprift-openapi.json
  format: json
  label: Sprift Property API
  slug: sprift-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
- filename: sprift-openapi.json
  format: json
  label: Sprift Property V2 API
  slug: sprift-property-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
- filename: sprift-openapi.json
  format: json
  label: Sprift Search API
  slug: sprift-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
- filename: sprift-openapi.json
  format: json
  label: Sprift Insider API
  slug: sprift-insider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
- filename: sprift-openapi.json
  format: json
  label: Sprift Report Share API
  slug: sprift-share-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
- filename: sprift-openapi.json
  format: json
  label: Sprift User API
  slug: sprift-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/openapi/sprift-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sprift.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: sprift.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sprift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sprift, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sprift
provider_slug: sprift
slug: sprift-domain-security
source_filename: sprift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sprift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sprift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprift/refs/heads/main/security/sprift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Data
- Property Listings
- Valuation
- AVM
- Land Registry
- Conveyancing
- Rentals
- Mortgage
---
