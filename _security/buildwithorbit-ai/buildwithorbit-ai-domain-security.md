---
api_specs:
- filename: buildwithorbit-ai-integrate-api-openapi.yml
  format: yaml
  label: buildwithorbit-ai Integrate API
  slug: buildwithorbit-ai-integrate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildwithorbit-ai/openapi/buildwithorbit-ai-integrate-api-openapi.yml
- filename: buildwithorbit-ai-search-api-openapi.yml
  format: yaml
  label: buildwithorbit-ai Search API
  slug: buildwithorbit-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildwithorbit-ai/openapi/buildwithorbit-ai-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: buildwithorbit.ai
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: buildwithorbit.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buildwithorbit Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for buildwithorbit-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: buildwithorbit-ai
provider_slug: buildwithorbit-ai
slug: buildwithorbit-ai-domain-security
source_filename: buildwithorbit-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buildwithorbit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buildwithorbit.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/buildwithorbit-ai/security/buildwithorbit-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- API-Discovery
- Integration
- MCP
- Postman
- Platform
---
