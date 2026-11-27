---
api_specs:
- filename: plaingateway-chat-completions-api-openapi.yml
  format: yaml
  label: plaingateway Chat Completions API
  slug: plaingateway-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plaingateway/openapi/plaingateway-chat-completions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: plaingateway.com
  spf: false
hosts:
- cert_expires: Jan 15 16:47:28 2027 GMT
  host: plaingateway.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: plaingateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for plaingateway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: plaingateway
provider_slug: plaingateway
slug: plaingateway-domain-security
source_filename: plaingateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plaingateway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 16:47:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: plaingateway.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/plaingateway/security/plaingateway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- LLM
- API Gateway
- OpenRouter-Alternative
- Free
---
