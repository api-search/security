---
api_specs:
- filename: nordax-ai-categories-api-openapi.yml
  format: yaml
  label: Nordax AI Categories API
  slug: nordax-ai-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nordax-ai/openapi/nordax-ai-categories-api-openapi.yml
- filename: nordax-ai-entities-api-openapi.yml
  format: yaml
  label: Nordax AI Entities API
  slug: nordax-ai-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nordax-ai/openapi/nordax-ai-entities-api-openapi.yml
- filename: nordax-ai-netp-api-openapi.yml
  format: yaml
  label: Nordax AI Netp API
  slug: nordax-ai-netp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nordax-ai/openapi/nordax-ai-netp-api-openapi.yml
- filename: nordax-ai-stats-api-openapi.yml
  format: yaml
  label: Nordax AI Stats API
  slug: nordax-ai-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nordax-ai/openapi/nordax-ai-stats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: nordax.ai
  spf: true
hosts:
- cert_expires: Jan 28 09:56:38 2027 GMT
  host: www.nordax.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 00:43:27 2027 GMT
  host: api.nordax.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Nordax AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nordax AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nordax AI
provider_slug: nordax-ai
slug: nordax-ai-domain-security
source_filename: nordax-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nordax.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 09:56:38 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.nordax.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 00:43:27 2027 GMT\n  hsts: null\ndomains:\n- domain: nordax.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/nordax-ai/security/nordax-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Identity
- Trust
- Platform
---
