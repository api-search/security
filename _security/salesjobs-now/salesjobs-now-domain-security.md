---
api_specs:
- filename: salesjobs-now-jobs-api-openapi.yml
  format: yaml
  label: SalesJobs.Now Jobs API
  slug: salesjobs-now-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/salesjobs-now/openapi/salesjobs-now-jobs-api-openapi.yml
- filename: salesjobs-now-pay-csv-api-openapi.yml
  format: yaml
  label: SalesJobs.Now Pay.csv API
  slug: salesjobs-now-pay-csv-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/salesjobs-now/openapi/salesjobs-now-pay-csv-api-openapi.yml
- filename: salesjobs-now-pay-json-api-openapi.yml
  format: yaml
  label: SalesJobs.Now Pay.json API
  slug: salesjobs-now-pay-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/salesjobs-now/openapi/salesjobs-now-pay-json-api-openapi.yml
- filename: salesjobs-now-roles-json-api-openapi.yml
  format: yaml
  label: SalesJobs.Now Roles.json API
  slug: salesjobs-now-roles-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/salesjobs-now/openapi/salesjobs-now-roles-json-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: salesjobs.now
  spf: false
hosts:
- cert_expires: Jan 28 13:28:03 2027 GMT
  host: salesjobs.now
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Salesjobs Now Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SalesJobs.Now, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: SalesJobs.Now
provider_slug: salesjobs-now
slug: salesjobs-now-domain-security
source_filename: salesjobs-now-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: salesjobs.now\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 13:28:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: salesjobs.now\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/salesjobs-now/security/salesjobs-now-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales
- Job
- Recruiting
- Data
---
