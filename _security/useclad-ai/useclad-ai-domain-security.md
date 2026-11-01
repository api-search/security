---
api_specs:
- filename: useclad-ai-openapi-generated.yml
  format: yaml
  label: Clad Labs API
  slug: useclad-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/useclad-ai/openapi/_ae-authored/useclad-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: useclad.ai
  spf: true
hosts:
- cert_expires: Jan  2 22:02:16 2027 GMT
  host: useclad.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Useclad Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clad Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clad Labs
provider_slug: useclad-ai
slug: useclad-ai-domain-security
source_filename: useclad-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: useclad.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 22:02:16 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: useclad.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/useclad-ai/security/useclad-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Support
- SaaS
- Automation
---
