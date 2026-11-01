---
api_specs:
- filename: aitraining-jobs-pay-csv-api-openapi.yml
  format: yaml
  label: AITraining.jobs Pay.csv API
  slug: aitraining-jobs-pay-csv-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitraining-jobs/openapi/aitraining-jobs-pay-csv-api-openapi.yml
- filename: aitraining-jobs-pay-json-api-openapi.yml
  format: yaml
  label: AITraining.jobs Pay.json API
  slug: aitraining-jobs-pay-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitraining-jobs/openapi/aitraining-jobs-pay-json-api-openapi.yml
- filename: aitraining-jobs-roles-json-api-openapi.yml
  format: yaml
  label: AITraining.jobs Roles.json API
  slug: aitraining-jobs-roles-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aitraining-jobs/openapi/aitraining-jobs-roles-json-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aitraining.jobs
  spf: false
hosts:
- cert_expires: Dec 12 20:32:15 2026 GMT
  host: aitraining.jobs
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aitraining Jobs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AITraining.jobs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AITraining.jobs
provider_slug: aitraining-jobs
slug: aitraining-jobs-domain-security
source_filename: aitraining-jobs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aitraining.jobs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 20:32:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aitraining.jobs\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aitraining-jobs/security/aitraining-jobs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Job
- Data
- Training
---
