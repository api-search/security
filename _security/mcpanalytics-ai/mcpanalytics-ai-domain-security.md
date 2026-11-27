---
api_specs:
- filename: mcpanalytics-ai-openapi-generated.yml
  format: yaml
  label: MCP Analytics API
  slug: mcpanalytics-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpanalytics-ai/openapi/_ae-authored/mcpanalytics-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mcpanalytics.ai
  spf: true
hosts:
- cert_expires: Jan  8 23:20:51 2027 GMT
  host: mcpanalytics.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCP Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCP Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MCP Analytics
provider_slug: mcpanalytics-ai
slug: mcpanalytics-ai-domain-security
source_filename: mcpanalytics-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpanalytics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:20:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mcpanalytics.ai\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mcpanalytics-ai/security/mcpanalytics-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Statistical Analysis
- Data Science
- Business Analytics
- Reproducible Analytics
- Custom Analytics
- Data Connectors
- AI Agent Integration
---
