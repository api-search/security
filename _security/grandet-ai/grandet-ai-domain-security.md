---
api_specs:
- filename: grandet-ai-openapi.yml
  format: yaml
  label: Grandet Anonymous Price Discovery API
  slug: grandet-anonymous-price-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grandet-ai/openapi/grandet-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: grandet.ai
  spf: false
hosts:
- cert_expires: Jan  4 08:58:31 2027 GMT
  host: grandet.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Grandet Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for grandet-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: grandet-ai
provider_slug: grandet-ai
slug: grandet-ai-domain-security
source_filename: grandet-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grandet.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 08:58:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: grandet.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/grandet-ai/security/grandet-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- LLM
- Pricing
- Data
---
