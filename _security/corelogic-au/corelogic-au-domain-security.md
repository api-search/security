---
api_specs:
- filename: corelogic-au-rp-inside-auth-example.postman_collection.json
  format: json
  label: CoreLogic Australia Access API
  slug: corelogic-au-access-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-rp-inside-auth-example.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Property Details API
  slug: corelogic-au-property-details-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Property Services API
  slug: corelogic-au-property-services-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Search API
  slug: corelogic-au-search-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia AVM API
  slug: corelogic-au-avm-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Auction API
  slug: corelogic-au-auction-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Statistics API
  slug: corelogic-au-statistics-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Charts API
  slug: corelogic-au-charts-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Property Timeline API
  slug: corelogic-au-property-timeline-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
- filename: corelogic-au-sample-sandbox.postman_collection.json
  format: json
  label: CoreLogic Australia Content API
  slug: corelogic-au-content-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/collections/corelogic-au-sample-sandbox.postman_collection.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cotality.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: corelogic.asia
  spf: true
hosts:
- cert_expires: Oct  7 04:27:56 2026 GMT
  host: www.cotality.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 06:29:41 2026 GMT
  host: developer.corelogic.asia
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 01:27:10 2026 GMT
  host: access.api.cotality.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corelogic Au Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoreLogic Australia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CoreLogic Australia
provider_slug: corelogic-au
slug: corelogic-au-domain-security
source_filename: corelogic-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cotality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:27:56 2026 GMT\n  hsts: false\n- host: developer.corelogic.asia\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 06:29:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: access.api.cotality.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 01:27:10 2026 GMT\n  hsts: null\ndomains:\n- domain: cotality.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: corelogic.asia\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corelogic-au/refs/heads/main/security/corelogic-au-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- Australia
- Property Data
- Valuation
- AVM
- PropTech
- Property Listings
- Rentals
- Auction Data
- Commercial Real Estate
- Mortgage
- Land Registry
- Cotality
- RP Data
---
