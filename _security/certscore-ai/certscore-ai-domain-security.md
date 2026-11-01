---
api_specs:
- filename: certscore-ai-auth-api-openapi.yml
  format: yaml
  label: certscore-ai Auth API
  slug: certscore-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-auth-api-openapi.yml
- filename: certscore-ai-diagnostics-api-openapi.yml
  format: yaml
  label: certscore-ai Diagnostics API
  slug: certscore-ai-diagnostics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-diagnostics-api-openapi.yml
- filename: certscore-ai-domains-api-openapi.yml
  format: yaml
  label: certscore-ai Domains API
  slug: certscore-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-domains-api-openapi.yml
- filename: certscore-ai-findings-api-openapi.yml
  format: yaml
  label: certscore-ai Findings API
  slug: certscore-ai-findings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-findings-api-openapi.yml
- filename: certscore-ai-pulse-api-openapi.yml
  format: yaml
  label: certscore-ai Pulse API
  slug: certscore-ai-pulse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-pulse-api-openapi.yml
- filename: certscore-ai-runtime-inventory-api-openapi.yml
  format: yaml
  label: certscore-ai Runtime Inventory API
  slug: certscore-ai-runtime-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-runtime-inventory-api-openapi.yml
- filename: certscore-ai-scans-api-openapi.yml
  format: yaml
  label: certscore-ai Scans API
  slug: certscore-ai-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certscore-ai/openapi/certscore-ai-scans-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: certscore.ai
  spf: true
hosts:
- cert_expires: Jan 13 07:11:13 2027 GMT
  host: certscore.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Certscore Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for certscore-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: certscore-ai
provider_slug: certscore-ai
slug: certscore-ai-domain-security
source_filename: certscore-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: certscore.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 07:11:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: certscore.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/certscore-ai/security/certscore-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Privacy
- Security
- Scanning
- Compliance
---
