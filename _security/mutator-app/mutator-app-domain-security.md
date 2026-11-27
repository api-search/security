---
api_specs:
- filename: mutator-app-analytics-api-openapi.yml
  format: yaml
  label: Mutator Analytics API
  slug: mutator-app-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-analytics-api-openapi.yml
- filename: mutator-app-approvals-api-openapi.yml
  format: yaml
  label: Mutator Approvals API
  slug: mutator-app-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-approvals-api-openapi.yml
- filename: mutator-app-assets-api-openapi.yml
  format: yaml
  label: Mutator Assets API
  slug: mutator-app-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-assets-api-openapi.yml
- filename: mutator-app-automations-api-openapi.yml
  format: yaml
  label: Mutator Automations API
  slug: mutator-app-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-automations-api-openapi.yml
- filename: mutator-app-generations-api-openapi.yml
  format: yaml
  label: Mutator Generations API
  slug: mutator-app-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-generations-api-openapi.yml
- filename: mutator-app-hooks-api-openapi.yml
  format: yaml
  label: Mutator Hooks API
  slug: mutator-app-hooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-hooks-api-openapi.yml
- filename: mutator-app-index-api-openapi.yml
  format: yaml
  label: Mutator Index API
  slug: mutator-app-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-index-api-openapi.yml
- filename: mutator-app-media-api-openapi.yml
  format: yaml
  label: Mutator Media API
  slug: mutator-app-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-media-api-openapi.yml
- filename: mutator-app-posts-api-openapi.yml
  format: yaml
  label: Mutator Posts API
  slug: mutator-app-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-posts-api-openapi.yml
- filename: mutator-app-runs-api-openapi.yml
  format: yaml
  label: Mutator Runs API
  slug: mutator-app-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-runs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mutator.app
  spf: true
hosts:
- cert_expires: Jan 11 04:09:45 2027 GMT
  host: mutator.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mutator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mutator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mutator
provider_slug: mutator-app
slug: mutator-app-domain-security
source_filename: mutator-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mutator.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 04:09:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mutator.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mutator-app/security/mutator-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Video
- UGC
- Marketing
- Platform
---
