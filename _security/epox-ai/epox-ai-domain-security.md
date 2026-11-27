---
api_specs:
- filename: epox-ai-openapi-generated.yml
  format: yaml
  label: Epox API
  slug: epox-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/epox-ai/openapi/_ae-authored/epox-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: epox.ai
  spf: true
hosts:
- cert_expires: Jan 29 18:04:19 2027 GMT
  host: epox.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Epox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Epox
provider_slug: epox-ai
slug: epox-ai-domain-security
source_filename: epox-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: epox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 18:04:19 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: epox.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/epox-ai/security/epox-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- E-Commerce
- Visuals
- Automation
- Platform
---
