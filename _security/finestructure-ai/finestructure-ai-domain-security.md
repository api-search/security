---
api_specs:
- filename: finestructure-ai-bridge-api-openapi.yml
  format: yaml
  label: Fine Structure Bridge API
  slug: finestructure-ai-bridge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-bridge-api-openapi.yml
- filename: finestructure-ai-discovery-api-openapi.yml
  format: yaml
  label: Fine Structure Discovery API
  slug: finestructure-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-discovery-api-openapi.yml
- filename: finestructure-ai-mcp-api-openapi.yml
  format: yaml
  label: Fine Structure MCP API
  slug: finestructure-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-mcp-api-openapi.yml
- filename: finestructure-ai-tools-api-openapi.yml
  format: yaml
  label: Fine Structure Tools API
  slug: finestructure-ai-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finestructure-ai/openapi/finestructure-ai-tools-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: finestructure.ai
  spf: true
hosts:
- cert_expires: Jan 19 10:42:33 2027 GMT
  host: finestructure.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fine Structure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fine Structure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fine Structure
provider_slug: finestructure-ai
slug: finestructure-ai-domain-security
source_filename: finestructure-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finestructure.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 10:42:33 2027 GMT\n  hsts: null\ndomains:\n- domain: finestructure.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/finestructure-ai/security/finestructure-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Automation
- Platform
- Integration
- Business
---
