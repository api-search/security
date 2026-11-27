---
api_specs:
- filename: byteask-ai-api-openapi.json
  format: json
  label: ByteAsk public status endpoints Api API
  slug: byteask-public-status-endpoints-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/byteask-ai/openapi/_original/byteask-ai-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: byteask.ai
  spf: true
hosts:
- cert_expires: Jan  7 10:03:05 2027 GMT
  host: byteask.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ByteAsk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ByteAsk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ByteAsk
provider_slug: byteask-ai
slug: byteask-ai-domain-security
source_filename: byteask-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: byteask.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 10:03:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: byteask.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/byteask-ai/security/byteask-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Coding
- C++
- Terminal
- Automation
---
