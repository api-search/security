---
api_specs:
- filename: chia-health-catalog-api-openapi.yml
  format: yaml
  label: Chia Health Catalog API
  slug: chia-health-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chia-health/openapi/chia-health-catalog-api-openapi.yml
- filename: chia-health-handoff-sessions-api-openapi.yml
  format: yaml
  label: Chia Health Handoff sessions API
  slug: chia-health-handoff-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chia-health/openapi/chia-health-handoff-sessions-api-openapi.yml
- filename: chia-health-settlements-api-openapi.yml
  format: yaml
  label: Chia Health Settlements API
  slug: chia-health-settlements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chia-health/openapi/chia-health-settlements-api-openapi.yml
- filename: chia-health-webhook-tests-api-openapi.yml
  format: yaml
  label: Chia Health Webhook tests API
  slug: chia-health-webhook-tests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chia-health/openapi/chia-health-webhook-tests-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chia.health
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: chia.health
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chia Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chia Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chia Health
provider_slug: chia-health
slug: chia-health-domain-security
source_filename: chia-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chia.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: chia.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chia-health/security/chia-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Telehealth
- Healthcare
- Peptides
- GLP-1
- Weight Loss
- Partner API
- MCP
---
