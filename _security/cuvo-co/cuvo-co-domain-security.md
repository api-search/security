---
api_specs:
- filename: cuvo-co-a2a-api-openapi.yml
  format: yaml
  label: Cuvo Health A2a API
  slug: cuvo-co-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-a2a-api-openapi.yml
- filename: cuvo-co-acp-api-openapi.yml
  format: yaml
  label: Cuvo Health Acp API
  slug: cuvo-co-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-acp-api-openapi.yml
- filename: cuvo-co-content-api-openapi.yml
  format: yaml
  label: Cuvo Health Content API
  slug: cuvo-co-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-content-api-openapi.yml
- filename: cuvo-co-discovery-api-openapi.yml
  format: yaml
  label: Cuvo Health Discovery API
  slug: cuvo-co-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-discovery-api-openapi.yml
- filename: cuvo-co-mcp-api-openapi.yml
  format: yaml
  label: Cuvo Health MCP API
  slug: cuvo-co-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-mcp-api-openapi.yml
- filename: cuvo-co-status-api-openapi.yml
  format: yaml
  label: Cuvo Health Status API
  slug: cuvo-co-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuvo-co/openapi/cuvo-co-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cuvo.co
  spf: true
hosts:
- cert_expires: Jan 23 22:48:28 2027 GMT
  host: cuvo.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cuvo Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cuvo Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cuvo Health
provider_slug: cuvo-co
slug: cuvo-co-domain-security
source_filename: cuvo-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cuvo.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 22:48:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cuvo.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cuvo-co/security/cuvo-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telehealth
- White‑Label Platform
- Pharmacy Fulfillment
- Brand Licensing
---
