---
api_specs:
- filename: direct-freight-boards-api-openapi.yml
  format: yaml
  label: Direct Freight Boards API
  slug: direct-freight-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/direct-freight/openapi/direct-freight-boards-api-openapi.yml
- filename: direct-freight-end-user-authentications-api-openapi.yml
  format: yaml
  label: Direct Freight End User Authentications API
  slug: direct-freight-end-user-authentications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/direct-freight/openapi/direct-freight-end-user-authentications-api-openapi.yml
- filename: direct-freight-locations-api-openapi.yml
  format: yaml
  label: Direct Freight Locations API
  slug: direct-freight-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/direct-freight/openapi/direct-freight-locations-api-openapi.yml
- filename: direct-freight-postings-api-openapi.yml
  format: yaml
  label: Direct Freight Postings API
  slug: direct-freight-postings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/direct-freight/openapi/direct-freight-postings-api-openapi.yml
- filename: direct-freight-profiles-api-openapi.yml
  format: yaml
  label: Direct Freight Profiles API
  slug: direct-freight-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/direct-freight/openapi/direct-freight-profiles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: directfreight.com
  spf: true
hosts:
- cert_expires: Jan 17 03:07:52 2027 GMT
  host: directfreight.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Direct Freight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Direct Freight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Direct Freight
provider_slug: direct-freight
slug: direct-freight-domain-security
source_filename: direct-freight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: directfreight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 03:07:52 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: directfreight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/direct-freight/security/direct-freight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Load Board
- Freight Brokers
- Shippers
- Carrier
- Owner Operators
- Freight Rate Tool
- Mileage Calculator
---
