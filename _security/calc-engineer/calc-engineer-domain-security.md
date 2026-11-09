---
api_specs:
- filename: calc-engineer-auth-api-openapi.yml
  format: yaml
  label: calc.engineer Auth API
  slug: calc-engineer-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-auth-api-openapi.yml
- filename: calc-engineer-catalog-api-openapi.yml
  format: yaml
  label: calc.engineer Catalog API
  slug: calc-engineer-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-catalog-api-openapi.yml
- filename: calc-engineer-docs-api-openapi.yml
  format: yaml
  label: calc.engineer Docs API
  slug: calc-engineer-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-docs-api-openapi.yml
- filename: calc-engineer-general-api-openapi.yml
  format: yaml
  label: calc.engineer General API
  slug: calc-engineer-general-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-general-api-openapi.yml
- filename: calc-engineer-homelab-api-openapi.yml
  format: yaml
  label: calc.engineer Homelab API
  slug: calc-engineer-homelab-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-homelab-api-openapi.yml
- filename: calc-engineer-mesh-api-openapi.yml
  format: yaml
  label: calc.engineer Mesh API
  slug: calc-engineer-mesh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-mesh-api-openapi.yml
- filename: calc-engineer-pcb-api-openapi.yml
  format: yaml
  label: calc.engineer Pcb API
  slug: calc-engineer-pcb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-pcb-api-openapi.yml
- filename: calc-engineer-power-api-openapi.yml
  format: yaml
  label: calc.engineer Power API
  slug: calc-engineer-power-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-power-api-openapi.yml
- filename: calc-engineer-rf-api-openapi.yml
  format: yaml
  label: calc.engineer Rf API
  slug: calc-engineer-rf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/calc-engineer/openapi/calc-engineer-rf-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: calc.engineer
  spf: false
hosts:
- cert_expires: Dec 23 14:59:36 2026 GMT
  host: calc.engineer
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Calc Engineer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for calc.engineer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: calc.engineer
provider_slug: calc-engineer
slug: calc-engineer-domain-security
source_filename: calc-engineer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calc.engineer\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 14:59:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: calc.engineer\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/calc-engineer/security/calc-engineer-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Engineering
- Simulation
- Calculator
---
