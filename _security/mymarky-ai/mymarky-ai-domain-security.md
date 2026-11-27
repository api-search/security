---
api_specs:
- filename: mymarky-ai-openapi-generated.yml
  format: yaml
  label: Marky API
  slug: mymarky-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mymarky-ai/openapi/_ae-authored/mymarky-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mymarky.ai
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: mymarky.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Marky Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marky, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Marky
provider_slug: mymarky-ai
slug: mymarky-ai-domain-security
source_filename: mymarky-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mymarky.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mymarky.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mymarky-ai/security/mymarky-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Social Media
- Marketing
- Small Business
- Automation
---
