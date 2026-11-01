---
api_specs:
- filename: convrgent-ai-openapi.json
  format: json
  label: Convrgent API
  slug: convrgent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convrgent-ai/openapi/_original/convrgent-ai-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: convrgent.ai
  spf: false
hosts:
- cert_expires: Dec  6 07:53:48 2026 GMT
  host: convrgent.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Convrgent Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for convrgent-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: convrgent-ai
provider_slug: convrgent-ai
slug: convrgent-ai-domain-security
source_filename: convrgent-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: convrgent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 07:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: convrgent.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/convrgent-ai/security/convrgent-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Personality-Intelligence
- x402
- Microservices
- API
---
