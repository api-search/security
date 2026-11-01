---
api_specs:
- filename: promptitude-openapi-generated.yml
  format: yaml
  label: Promptitude API
  slug: promptitude-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptitude/openapi/_ae-authored/promptitude-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: promptitude.io
  spf: true
hosts:
- cert_expires: Nov 22 08:00:10 2026 GMT
  host: promptitude.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Promptitude Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Promptitude, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Promptitude
provider_slug: promptitude
slug: promptitude-domain-security
source_filename: promptitude-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: promptitude.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 08:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: promptitude.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/promptitude/security/promptitude-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- No-Code
- Prompt Engineering
- Automation
---
