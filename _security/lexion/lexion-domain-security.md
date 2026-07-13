---
api_specs:
- filename: lexion-openapi.yml
  format: yaml
  label: Lexion Contract Repository
  slug: contract-repository
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexion/refs/heads/main/openapi/lexion-openapi.yml
- filename: lexion-openapi.yml
  format: yaml
  label: Lexion Extraction & Insights
  slug: extraction-insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexion/refs/heads/main/openapi/lexion-openapi.yml
- filename: lexion-openapi.yml
  format: yaml
  label: Lexion Workflows
  slug: workflows
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexion/refs/heads/main/openapi/lexion-openapi.yml
- filename: lexion-openapi.yml
  format: yaml
  label: Lexion Integrations
  slug: integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lexion/refs/heads/main/openapi/lexion-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lexion.ai
  spf: true
hosts:
- cert_expires: Sep 29 00:23:44 2026 GMT
  host: www.lexion.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lexion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lexion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lexion
provider_slug: lexion
slug: lexion-domain-security
source_filename: lexion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lexion.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 00:23:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lexion.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lexion/refs/heads/main/security/lexion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Contract Management
- CLM
- AI
- Legal Tech
- Document Extraction
- Workflow
---
