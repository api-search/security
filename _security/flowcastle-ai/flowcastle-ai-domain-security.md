---
api_specs:
- filename: flowcastle-ai-openapi-generated.yml
  format: yaml
  label: FlowCastle API
  slug: flowcastle-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flowcastle-ai/openapi/_ae-authored/flowcastle-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flowcastle.ai
  spf: true
hosts:
- cert_expires: Jan 11 10:30:30 2027 GMT
  host: flowcastle.ai
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FlowCastle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlowCastle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FlowCastle
provider_slug: flowcastle-ai
slug: flowcastle-ai-domain-security
source_filename: flowcastle-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowcastle.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 10:30:30 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: flowcastle.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flowcastle-ai/security/flowcastle-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Bot Builder
- Telegram
- No-Code
- Artificial Intelligence
---
