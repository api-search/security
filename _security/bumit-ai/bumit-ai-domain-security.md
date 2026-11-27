---
api_specs:
- filename: bumit-ai-v1-openapi.json
  format: json
  label: BUMIT API V1 API
  slug: bumit-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bumit-ai/openapi/_original/bumit-ai-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bumit.ai
  spf: true
hosts:
- cert_expires: Dec 22 18:11:34 2026 GMT
  host: bumit.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BUMIT Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BUMIT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BUMIT
provider_slug: bumit-ai
slug: bumit-ai-domain-security
source_filename: bumit-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bumit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 18:11:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bumit.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bumit-ai/security/bumit-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Trust
- Verification
- Swiss
---
