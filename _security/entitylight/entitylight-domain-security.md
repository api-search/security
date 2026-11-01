---
api_specs:
- filename: entitylight-business-searches-api-openapi.yml
  format: yaml
  label: Entitylight Business Searches API
  slug: entitylight-business-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entitylight/openapi/entitylight-business-searches-api-openapi.yml
- filename: entitylight-lookups-api-openapi.yml
  format: yaml
  label: Entitylight Lookups API
  slug: entitylight-lookups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entitylight/openapi/entitylight-lookups-api-openapi.yml
- filename: entitylight-ofac-screenings-api-openapi.yml
  format: yaml
  label: Entitylight Ofac Screenings API
  slug: entitylight-ofac-screenings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entitylight/openapi/entitylight-ofac-screenings-api-openapi.yml
- filename: entitylight-ucc-searches-api-openapi.yml
  format: yaml
  label: Entitylight Ucc Searches API
  slug: entitylight-ucc-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entitylight/openapi/entitylight-ucc-searches-api-openapi.yml
- filename: entitylight-usage-api-openapi.yml
  format: yaml
  label: Entitylight Usage API
  slug: entitylight-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entitylight/openapi/entitylight-usage-api-openapi.yml
- filename: entitylight-watches-api-openapi.yml
  format: yaml
  label: Entitylight Watches API
  slug: entitylight-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entitylight/openapi/entitylight-watches-api-openapi.yml
- filename: entitylight-webhook-api-openapi.yml
  format: yaml
  label: Entitylight Webhook API
  slug: entitylight-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entitylight/openapi/entitylight-webhook-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: entitylight.com
  spf: true
hosts:
- cert_expires: Jan 25 09:28:57 2027 GMT
  host: entitylight.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Entitylight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entitylight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Entitylight
provider_slug: entitylight
slug: entitylight-domain-security
source_filename: entitylight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: entitylight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 09:28:57 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: entitylight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/entitylight/security/entitylight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Business
- API
- UCC
- Litigation
- Monitoring
---
