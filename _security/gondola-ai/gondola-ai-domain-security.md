---
api_specs:
- filename: gondola-ai-infrastructure-api-openapi.yml
  format: yaml
  label: Gondola Infrastructure API
  slug: gondola-ai-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gondola-ai/openapi/gondola-ai-infrastructure-api-openapi.yml
- filename: gondola-ai-partner-search-api-openapi.yml
  format: yaml
  label: Gondola Partner Search API
  slug: gondola-ai-partner-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gondola-ai/openapi/gondola-ai-partner-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gondola.ai
  spf: true
hosts:
- cert_expires: Feb  1 11:57:02 2027 GMT
  host: gondola.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gondola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gondola, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Gondola
provider_slug: gondola-ai
slug: gondola-ai-domain-security
source_filename: gondola-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gondola.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 11:57:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gondola.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gondola-ai/security/gondola-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- Rewards
- Hotel Booking
- Fintech
- Consumer
---
