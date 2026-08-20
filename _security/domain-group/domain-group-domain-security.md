---
api_specs:
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Address Suggestions API
  slug: domain-address-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Agents & Listings API
  slug: domain-agents-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Campaign API
  slug: domain-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Campaign API - Preview
  slug: domain-campaign-api-preview
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Listings Management API
  slug: domain-listings-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Price Estimation API
  slug: domain-price-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Properties & Locations API
  slug: domain-properties-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Property Enrichment API
  slug: domain-property-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Property Package API
  slug: domain-property-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain PropertyRadar API
  slug: domain-propertyradar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Rental AVM API
  slug: domain-rental-avm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Schools Data API
  slug: domain-schools-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
- filename: domain-group-openapi-latest.json
  format: json
  label: Domain Webhooks API
  slug: domain-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/openapi/domain-group-openapi-latest.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: domain.com.au
  spf: true
hosts:
- cert_expires: Aug 20 19:01:42 2026 GMT
  host: www.domain.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  3 23:59:59 2026 GMT
  host: developer.domain.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 15:49:35 2026 GMT
  host: api.domain.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Domain Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domain Group, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Domain Group
provider_slug: domain-group
slug: domain-group-domain-security
source_filename: domain-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.domain.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 19:01:42 2026 GMT\n  hsts: null\n- host: developer.domain.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 23:59:59 2026 GMT\n  hsts: false\n- host: api.domain.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:49:35 2026 GMT\n  hsts: null\ndomains:\n- domain: domain.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domain-group/refs/heads/main/security/domain-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real-Estate
- Australia
- Property Listings
- Property Data
- Valuation
- AVM
- Rentals
- Listing Management
- PropTech
- Portal Marketplace
---
