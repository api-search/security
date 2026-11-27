---
api_specs:
- filename: mako-ai-openapi-generated.yml
  format: yaml
  label: Mako API
  slug: mako-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mako-ai/openapi/_ae-authored/mako-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mako.ai
  spf: false
hosts:
- cert_expires: Feb  3 09:20:42 2027 GMT
  host: mako.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mako Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mako, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Mako
provider_slug: mako-ai
slug: mako-ai-domain-security
source_filename: mako-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mako.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 09:20:42 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mako.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mako-ai/security/mako-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Data
- Open Source
- ETL
- Platform
---
