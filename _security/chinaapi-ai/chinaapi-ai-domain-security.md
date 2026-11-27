---
api_specs:
- filename: chinaapi-ai-openapi-generated.yml
  format: yaml
  label: ChinaAPI API
  slug: chinaapi-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chinaapi-ai/openapi/_ae-authored/chinaapi-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chinaapi.ai
  spf: true
hosts:
- cert_expires: Jan 10 11:34:31 2027 GMT
  host: chinaapi.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 11:34:31 2027 GMT
  host: dash.chinaapi.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: ChinaAPI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ChinaAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ChinaAPI
provider_slug: chinaapi-ai
slug: chinaapi-ai-domain-security
source_filename: chinaapi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chinaapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 11:34:31 2027 GMT\n  hsts: false\n- host: dash.chinaapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 11:34:31 2027 GMT\n  hsts: false\ndomains:\n- domain: chinaapi.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chinaapi-ai/security/chinaapi-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- LLM
- API Gateway
- OpenAI-Compatible
- Video Generation
- Image Generation
- Speech
- MCP
- China
---
