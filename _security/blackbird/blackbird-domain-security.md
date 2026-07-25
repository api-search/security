---
api_specs:
- filename: blackbird-app-api-openapi.yml
  format: yaml
  label: Blackbird App API
  slug: blackbird-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-app-api-openapi.yml
- filename: blackbird-challenges-api-openapi.yml
  format: yaml
  label: Blackbird Challenges API
  slug: blackbird-challenges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-challenges-api-openapi.yml
- filename: blackbird-check-ins-api-openapi.yml
  format: yaml
  label: Blackbird Check-ins API
  slug: blackbird-check-ins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-check-ins-api-openapi.yml
- filename: blackbird-locations-api-openapi.yml
  format: yaml
  label: Blackbird Locations API
  slug: blackbird-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-locations-api-openapi.yml
- filename: blackbird-memberships-api-openapi.yml
  format: yaml
  label: Blackbird Memberships API
  slug: blackbird-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-memberships-api-openapi.yml
- filename: blackbird-payments-api-openapi.yml
  format: yaml
  label: Blackbird Payments API
  slug: blackbird-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-payments-api-openapi.yml
- filename: blackbird-restaurants-api-openapi.yml
  format: yaml
  label: Blackbird Restaurants API
  slug: blackbird-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-restaurants-api-openapi.yml
- filename: blackbird-rewards-api-openapi.yml
  format: yaml
  label: Blackbird Rewards API
  slug: blackbird-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-rewards-api-openapi.yml
- filename: blackbird-specials-api-openapi.yml
  format: yaml
  label: Blackbird Specials API
  slug: blackbird-specials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-specials-api-openapi.yml
- filename: blackbird-users-api-openapi.yml
  format: yaml
  label: Blackbird Users API
  slug: blackbird-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/openapi/blackbird-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blackbird.xyz
  spf: true
hosts:
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: blackbird.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: api.staging.blackbird.xyz
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Blackbird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blackbird, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blackbird
provider_slug: blackbird
slug: blackbird-domain-security
source_filename: blackbird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blackbird.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: false\n- host: api.staging.blackbird.xyz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: blackbird.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackbird/refs/heads/main/security/blackbird-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Restaurants
- Loyalty
- Payments
- Dining
- Membership
- Crypto
- Blockchain
- Web3
---
