---
api_specs:
- filename: autohost-accounts-api-openapi.yml
  format: yaml
  label: Autohost Accounts API
  slug: autohost-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-accounts-api-openapi.yml
- filename: autohost-background-check-api-openapi.yml
  format: yaml
  label: Autohost Background Check API
  slug: autohost-background-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-background-check-api-openapi.yml
- filename: autohost-fraud-api-openapi.yml
  format: yaml
  label: Autohost Fraud API
  slug: autohost-fraud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-fraud-api-openapi.yml
- filename: autohost-idcheck-api-openapi.yml
  format: yaml
  label: Autohost Idcheck API
  slug: autohost-idcheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-idcheck-api-openapi.yml
- filename: autohost-listings-api-openapi.yml
  format: yaml
  label: Autohost Listings API
  slug: autohost-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-listings-api-openapi.yml
- filename: autohost-lookup-api-openapi.yml
  format: yaml
  label: Autohost Lookup API
  slug: autohost-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-lookup-api-openapi.yml
- filename: autohost-reservations-api-openapi.yml
  format: yaml
  label: Autohost Reservations API
  slug: autohost-reservations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-reservations-api-openapi.yml
- filename: autohost-validate-api-openapi.yml
  format: yaml
  label: Autohost Validate API
  slug: autohost-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autohost/openapi/autohost-validate-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: autohost.ai
  spf: true
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: autohost.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autohost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autohost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Autohost
provider_slug: autohost
slug: autohost-domain-security
source_filename: autohost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autohost.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: autohost.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/autohost/security/autohost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IdentityVerification
- BackgroundCheck
- FraudDetection
- Hospitality
- RealEstate
---
