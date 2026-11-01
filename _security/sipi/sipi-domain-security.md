---
api_specs:
- filename: sipi-agents-api-openapi.yml
  format: yaml
  label: GitDealFlow Agents API
  slug: sipi-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-agents-api-openapi.yml
- filename: sipi-approvals-api-openapi.yml
  format: yaml
  label: GitDealFlow Approvals API
  slug: sipi-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-approvals-api-openapi.yml
- filename: sipi-budget-api-openapi.yml
  format: yaml
  label: GitDealFlow Budget API
  slug: sipi-budget-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-budget-api-openapi.yml
- filename: sipi-evaluate-api-openapi.yml
  format: yaml
  label: GitDealFlow Evaluate API
  slug: sipi-evaluate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-evaluate-api-openapi.yml
- filename: sipi-rules-api-openapi.yml
  format: yaml
  label: GitDealFlow Rules API
  slug: sipi-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-rules-api-openapi.yml
- filename: sipi-system-api-openapi.yml
  format: yaml
  label: GitDealFlow System API
  slug: sipi-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sipi/openapi/sipi-system-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sipi.bot
  spf: true
hosts:
- cert_expires: Dec  5 11:57:32 2026 GMT
  host: sipi.bot
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sipi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GitDealFlow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GitDealFlow
provider_slug: sipi
slug: sipi-domain-security
source_filename: sipi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sipi.bot\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 11:57:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sipi.bot\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/sipi/security/sipi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Finance
- Security
- Automation
- Software-as-a-Service
---
