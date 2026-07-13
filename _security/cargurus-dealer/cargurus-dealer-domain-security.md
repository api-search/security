---
api_specs:
- filename: cargurus-dealer-openapi.yml
  format: yaml
  label: CarGurus Car Selector API
  slug: cargurus-car-selector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargurus-dealer/refs/heads/main/openapi/cargurus-dealer-openapi.yml
- filename: cargurus-dealer-openapi.yml
  format: yaml
  label: CarGurus Instant Market Value API
  slug: cargurus-instant-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargurus-dealer/refs/heads/main/openapi/cargurus-dealer-openapi.yml
- filename: cargurus-dealer-openapi.yml
  format: yaml
  label: CarGurus Dealer Reviews API
  slug: cargurus-dealer-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargurus-dealer/refs/heads/main/openapi/cargurus-dealer-openapi.yml
- filename: cargurus-dealer-openapi.yml
  format: yaml
  label: CarGurus Dealer Stats API
  slug: cargurus-dealer-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cargurus-dealer/refs/heads/main/openapi/cargurus-dealer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cargurus.com
  spf: true
hosts:
- cert_expires: Jan 10 14:58:38 2027 GMT
  host: www.cargurus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cargurus Dealer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarGurus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CarGurus
provider_slug: cargurus-dealer
slug: cargurus-dealer-domain-security
source_filename: cargurus-dealer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cargurus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 14:58:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cargurus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargurus-dealer/refs/heads/main/security/cargurus-dealer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Marketplace
- Car Listings
- Dealer
- Vehicle Pricing
- Reviews
- Inventory
---
