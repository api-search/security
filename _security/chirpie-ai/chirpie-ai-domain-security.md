---
api_specs:
- filename: chirpie-ai-openapi-generated.yml
  format: yaml
  label: Chirpie API
  slug: chirpie-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chirpie-ai/openapi/_ae-authored/chirpie-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chirpie.ai
  spf: true
hosts:
- cert_expires: Dec 19 09:59:12 2026 GMT
  host: chirpie.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chirpie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chirpie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chirpie
provider_slug: chirpie-ai
slug: chirpie-ai-domain-security
source_filename: chirpie-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chirpie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 09:59:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chirpie.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chirpie-ai/security/chirpie-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Media
- Social Media Posting
- Scheduling
- MCP
- AI Agents
- Analytics
---
