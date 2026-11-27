---
api_specs:
- filename: fiuto-ai-openapi-generated.yml
  format: yaml
  label: Fiuto API
  slug: fiuto-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fiuto-ai/openapi/_ae-authored/fiuto-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fiuto.ai
  spf: true
hosts:
- cert_expires: Feb  3 00:22:10 2027 GMT
  host: fiuto.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fiuto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fiuto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fiuto
provider_slug: fiuto-ai
slug: fiuto-ai-domain-security
source_filename: fiuto-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fiuto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 00:22:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fiuto.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fiuto-ai/security/fiuto-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- User Research
- Software-as-a-Service
- Artificial Intelligence
- No-Code
- Startups
---
