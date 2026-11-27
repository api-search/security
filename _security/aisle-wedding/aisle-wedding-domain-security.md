---
api_specs:
- filename: aisle-wedding-dress-codes-api-openapi.yml
  format: yaml
  label: Aisle Dress codes API
  slug: aisle-wedding-dress-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-dress-codes-api-openapi.yml
- filename: aisle-wedding-events-api-openapi.yml
  format: yaml
  label: Aisle Events API
  slug: aisle-wedding-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-events-api-openapi.yml
- filename: aisle-wedding-guest-access-api-openapi.yml
  format: yaml
  label: Aisle Guest access API
  slug: aisle-wedding-guest-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-guest-access-api-openapi.yml
- filename: aisle-wedding-guest-content-api-openapi.yml
  format: yaml
  label: Aisle Guest content API
  slug: aisle-wedding-guest-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-guest-content-api-openapi.yml
- filename: aisle-wedding-guests-api-openapi.yml
  format: yaml
  label: Aisle Guests API
  slug: aisle-wedding-guests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-guests-api-openapi.yml
- filename: aisle-wedding-media-api-openapi.yml
  format: yaml
  label: Aisle Media API
  slug: aisle-wedding-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-media-api-openapi.yml
- filename: aisle-wedding-meta-api-openapi.yml
  format: yaml
  label: Aisle Meta API
  slug: aisle-wedding-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-meta-api-openapi.yml
- filename: aisle-wedding-parties-api-openapi.yml
  format: yaml
  label: Aisle Parties API
  slug: aisle-wedding-parties-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-parties-api-openapi.yml
- filename: aisle-wedding-payments-api-openapi.yml
  format: yaml
  label: Aisle Payments API
  slug: aisle-wedding-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-payments-api-openapi.yml
- filename: aisle-wedding-payouts-api-openapi.yml
  format: yaml
  label: Aisle Payouts API
  slug: aisle-wedding-payouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-payouts-api-openapi.yml
- filename: aisle-wedding-recommendations-api-openapi.yml
  format: yaml
  label: Aisle Recommendations API
  slug: aisle-wedding-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-recommendations-api-openapi.yml
- filename: aisle-wedding-registry-api-openapi.yml
  format: yaml
  label: Aisle Registry API
  slug: aisle-wedding-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-registry-api-openapi.yml
- filename: aisle-wedding-rsvp-api-openapi.yml
  format: yaml
  label: Aisle RSVP API
  slug: aisle-wedding-rsvp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-rsvp-api-openapi.yml
- filename: aisle-wedding-site-api-openapi.yml
  format: yaml
  label: Aisle Site API
  slug: aisle-wedding-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-site-api-openapi.yml
- filename: aisle-wedding-statistics-api-openapi.yml
  format: yaml
  label: Aisle Statistics API
  slug: aisle-wedding-statistics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-statistics-api-openapi.yml
- filename: aisle-wedding-stays-api-openapi.yml
  format: yaml
  label: Aisle Stays API
  slug: aisle-wedding-stays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-stays-api-openapi.yml
- filename: aisle-wedding-travel-api-openapi.yml
  format: yaml
  label: Aisle Travel API
  slug: aisle-wedding-travel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-travel-api-openapi.yml
- filename: aisle-wedding-wedding-api-openapi.yml
  format: yaml
  label: Aisle Wedding API
  slug: aisle-wedding-wedding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aisle-wedding/openapi/aisle-wedding-wedding-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aisle.wedding
  spf: true
hosts:
- cert_expires: Dec 11 03:22:06 2026 GMT
  host: aisle.wedding
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aisle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aisle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aisle
provider_slug: aisle-wedding
slug: aisle-wedding-domain-security
source_filename: aisle-wedding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aisle.wedding\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 03:22:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aisle.wedding\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aisle-wedding/security/aisle-wedding-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wedding
- Planning
- Software-as-a-Service
- Marketplace
---
