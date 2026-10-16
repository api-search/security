---
api_specs:
- filename: tradera-auth-api-openapi.yml
  format: yaml
  label: Tradera Auth API
  slug: tradera-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-auth-api-openapi.yml
- filename: tradera-buyer-api-openapi.yml
  format: yaml
  label: Tradera Buyer API
  slug: tradera-buyer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-buyer-api-openapi.yml
- filename: tradera-categories-api-openapi.yml
  format: yaml
  label: Tradera Categories API
  slug: tradera-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-categories-api-openapi.yml
- filename: tradera-items-api-openapi.yml
  format: yaml
  label: Tradera Items API
  slug: tradera-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-items-api-openapi.yml
- filename: tradera-listings-api-openapi.yml
  format: yaml
  label: Tradera Listings API
  slug: tradera-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-listings-api-openapi.yml
- filename: tradera-orders-api-openapi.yml
  format: yaml
  label: Tradera Orders API
  slug: tradera-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-orders-api-openapi.yml
- filename: tradera-program-api-openapi.yml
  format: yaml
  label: Tradera Program API
  slug: tradera-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-program-api-openapi.yml
- filename: tradera-reference-data-api-openapi.yml
  format: yaml
  label: Tradera Reference Data API
  slug: tradera-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-reference-data-api-openapi.yml
- filename: tradera-search-api-openapi.yml
  format: yaml
  label: Tradera Search API
  slug: tradera-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-search-api-openapi.yml
- filename: tradera-tradera-api-services-core-api-openapi.yml
  format: yaml
  label: Tradera Tradera.Api.Services.Core API
  slug: tradera-tradera-api-services-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-tradera-api-services-core-api-openapi.yml
- filename: tradera-users-api-openapi.yml
  format: yaml
  label: Tradera Users API
  slug: tradera-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/openapi/tradera-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tradera.com
  spf: true
hosts:
- cert_expires: Jan  7 10:24:09 2027 GMT
  host: tradera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tradera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tradera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tradera
provider_slug: tradera
slug: tradera-domain-security
source_filename: tradera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tradera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 10:24:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tradera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradera/refs/heads/main/security/tradera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- E-commerce
- Secondhand
- Auctions
- Sweden
---
