---
api_specs:
- filename: collager-ai-account-api-openapi.yml
  format: yaml
  label: Collager.ai Account API
  slug: collager-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/collager-ai/openapi/collager-ai-account-api-openapi.yml
- filename: collager-ai-collages-api-openapi.yml
  format: yaml
  label: Collager.ai Collages API
  slug: collager-ai-collages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/collager-ai/openapi/collager-ai-collages-api-openapi.yml
- filename: collager-ai-mosaics-api-openapi.yml
  format: yaml
  label: Collager.ai Mosaics API
  slug: collager-ai-mosaics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/collager-ai/openapi/collager-ai-mosaics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: collager.ai
  spf: true
hosts:
- cert_expires: Jan 11 08:44:19 2027 GMT
  host: collager.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Collager.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collager.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Collager.ai
provider_slug: collager-ai
slug: collager-ai-domain-security
source_filename: collager-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: collager.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 08:44:19 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: collager.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/collager-ai/security/collager-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Photo Mosaic
- Photo Collage
- Image Generation
- Artificial Intelligence
- MCP
- Photography
---
