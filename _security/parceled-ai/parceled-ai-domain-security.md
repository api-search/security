---
api_specs:
- filename: parceled-ai-account-api-openapi.yml
  format: yaml
  label: parceled-ai Account API
  slug: parceled-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parceled-ai/openapi/parceled-ai-account-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parceled.ai
  spf: true
hosts:
- cert_expires: Jan  4 13:38:18 2027 GMT
  host: parceled.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Parceled Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for parceled-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: parceled-ai
provider_slug: parceled-ai
slug: parceled-ai-domain-security
source_filename: parceled-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parceled.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 13:38:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: parceled.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/parceled-ai/security/parceled-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- RealEstate
- DataAPI
- Mapping
- AI
---
