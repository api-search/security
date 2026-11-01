---
api_specs:
- filename: hacktron-rest-api-cost-estimations-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Cost Estimations API
  slug: hacktron-rest-api-cost-estimations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-cost-estimations-api-openapi.yml
- filename: hacktron-rest-api-findings-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Findings API
  slug: hacktron-rest-api-findings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-findings-api-openapi.yml
- filename: hacktron-rest-api-hfw-api-openapi.yml
  format: yaml
  label: Hacktron REST API - HFW API
  slug: hacktron-rest-api-hfw-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-hfw-api-openapi.yml
- filename: hacktron-rest-api-repos-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Repos API
  slug: hacktron-rest-api-repos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-repos-api-openapi.yml
- filename: hacktron-rest-api-scans-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Scans API
  slug: hacktron-rest-api-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-scans-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hacktron.ai
  spf: true
hosts:
- cert_expires: Dec 12 21:28:26 2026 GMT
  host: www.hacktron.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hacktron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hacktron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hacktron
provider_slug: hacktron
slug: hacktron-domain-security
source_filename: hacktron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hacktron.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 21:28:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hacktron.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hacktron/security/hacktron-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Automation
- Integration
- IoT
- Enterprise
---
