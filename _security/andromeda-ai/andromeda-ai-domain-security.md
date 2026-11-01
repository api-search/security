---
api_specs:
- filename: andromeda-ai-openapi-generated.yml
  format: yaml
  label: Andromeda API
  slug: andromeda-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/andromeda-ai/openapi/_ae-authored/andromeda-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: andromeda.ai
  spf: true
hosts:
- cert_expires: Jan 19 12:18:21 2027 GMT
  host: andromeda.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Andromeda Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andromeda, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Andromeda
provider_slug: andromeda-ai
slug: andromeda-ai-domain-security
source_filename: andromeda-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: andromeda.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 12:18:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: andromeda.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/andromeda-ai/security/andromeda-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Cloud
- Platform
- Machine-Learning
- Enterprise
---
