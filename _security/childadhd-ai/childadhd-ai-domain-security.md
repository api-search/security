---
api_specs:
- filename: childadhd-ai-articles-api-openapi.yml
  format: yaml
  label: ADHD in Children Articles API
  slug: childadhd-ai-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/childadhd-ai/openapi/childadhd-ai-articles-api-openapi.yml
- filename: childadhd-ai-mcp-api-openapi.yml
  format: yaml
  label: ADHD in Children MCP API
  slug: childadhd-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/childadhd-ai/openapi/childadhd-ai-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: childadhd.ai
  spf: false
hosts:
- cert_expires: Jan 16 06:06:50 2027 GMT
  host: childadhd.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ADHD in Children Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADHD in Children, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: ADHD in Children
provider_slug: childadhd-ai
slug: childadhd-ai-domain-security
source_filename: childadhd-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: childadhd.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 06:06:50 2027 GMT\n  hsts: false\ndomains:\n- domain: childadhd.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/childadhd-ai/security/childadhd-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- ADHD
- Pediatric Mental Health
- Parenting
- Health Information
- Behavioral Health
- MCP
- content-api
---
