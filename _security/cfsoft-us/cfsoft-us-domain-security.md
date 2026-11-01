---
api_specs:
- filename: cfsoft-us-batch-api-openapi.yml
  format: yaml
  label: cfsoft-us Batch API
  slug: cfsoft-us-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cfsoft-us/openapi/cfsoft-us-batch-api-openapi.yml
- filename: cfsoft-us-check-api-openapi.yml
  format: yaml
  label: cfsoft-us Check API
  slug: cfsoft-us-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cfsoft-us/openapi/cfsoft-us-check-api-openapi.yml
- filename: cfsoft-us-health-api-openapi.yml
  format: yaml
  label: cfsoft-us Health API
  slug: cfsoft-us-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cfsoft-us/openapi/cfsoft-us-health-api-openapi.yml
- filename: cfsoft-us-report-api-openapi.yml
  format: yaml
  label: cfsoft-us Report API
  slug: cfsoft-us-report-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cfsoft-us/openapi/cfsoft-us-report-api-openapi.yml
- filename: cfsoft-us-well-known-api-openapi.yml
  format: yaml
  label: cfsoft-us .well Known API
  slug: cfsoft-us-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cfsoft-us/openapi/cfsoft-us-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cfsoft.us
  spf: false
hosts:
- cert_expires: Dec 11 19:53:27 2026 GMT
  host: cfsoft.us
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cfsoft Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for cfsoft-us, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: cfsoft-us
provider_slug: cfsoft-us
slug: cfsoft-us-domain-security
source_filename: cfsoft-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cfsoft.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 19:53:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cfsoft.us\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cfsoft-us/security/cfsoft-us-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- API
- AI
- Finance
- Legal
---
