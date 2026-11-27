---
api_specs:
- filename: edgaze-ai-runs-api-openapi.yml
  format: yaml
  label: Edgaze Runs API
  slug: edgaze-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgaze-ai/openapi/edgaze-ai-runs-api-openapi.yml
- filename: edgaze-ai-workflows-api-openapi.yml
  format: yaml
  label: Edgaze Workflows API
  slug: edgaze-ai-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edgaze-ai/openapi/edgaze-ai-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edgaze.ai
  spf: true
hosts:
- cert_expires: Dec  9 11:27:45 2026 GMT
  host: edgaze.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Edgaze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edgaze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Edgaze
provider_slug: edgaze-ai
slug: edgaze-ai-domain-security
source_filename: edgaze-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edgaze.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 11:27:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: edgaze.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/edgaze-ai/security/edgaze-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- AI Workflows
- Creator Program
- Per‑run Pricing
- Workflow Studio
---
