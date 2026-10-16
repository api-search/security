---
api_specs:
- filename: airdna-market-data-api-openapi.yml
  format: yaml
  label: AirDNA Market Data API
  slug: airdna-market-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-market-data-api-openapi.yml
- filename: airdna-rentalizer-api-openapi.yml
  format: yaml
  label: AirDNA Rentalizer API
  slug: airdna-rentalizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-rentalizer-api-openapi.yml
- filename: airdna-rentalizer-lead-gen-api-openapi.yml
  format: yaml
  label: AirDNA Rentalizer Lead Gen API
  slug: airdna-rentalizer-lead-gen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-rentalizer-lead-gen-api-openapi.yml
- filename: airdna-smart-rates-api-openapi.yml
  format: yaml
  label: AirDNA Smart Rates API
  slug: airdna-smart-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-smart-rates-api-openapi.yml
- filename: airdna-str-listing-data-api-openapi.yml
  format: yaml
  label: AirDNA STR Listing Data API
  slug: airdna-str-listing-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-str-listing-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airdna.co
  spf: true
hosts:
- cert_expires: Nov 21 22:12:27 2026 GMT
  host: www.airdna.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 22:12:27 2026 GMT
  host: docs.airdna.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: api.airdna.co
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Airdna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AirDNA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AirDNA
provider_slug: airdna
slug: airdna-domain-security
source_filename: airdna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.airdna.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 22:12:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.airdna.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 22:12:27 2026 GMT\n  hsts: false\n- host: api.airdna.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: airdna.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/security/airdna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Short-Term Rental
- Vacation Rentals
- Market Data
- Real Estate
- Analytics
---
