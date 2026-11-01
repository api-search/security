---
api_specs:
- filename: tunova-ai-generation-api-openapi.yml
  format: yaml
  label: tunova-ai Generation API
  slug: tunova-ai-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tunova-ai/openapi/tunova-ai-generation-api-openapi.yml
- filename: tunova-ai-jobs-api-openapi.yml
  format: yaml
  label: tunova-ai Jobs API
  slug: tunova-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tunova-ai/openapi/tunova-ai-jobs-api-openapi.yml
- filename: tunova-ai-utility-api-openapi.yml
  format: yaml
  label: tunova-ai Utility API
  slug: tunova-ai-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tunova-ai/openapi/tunova-ai-utility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tunova.ai
  spf: true
hosts:
- cert_expires: Jan  7 10:41:56 2027 GMT
  host: tunova.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tunova Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tunova-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: tunova-ai
provider_slug: tunova-ai
slug: tunova-ai-domain-security
source_filename: tunova-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tunova.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 10:41:56 2027 GMT\n  hsts: false\ndomains:\n- domain: tunova.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tunova-ai/security/tunova-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Music
- Audio
- Suno
- TokenizedAPI
- REST
- MCP
---
