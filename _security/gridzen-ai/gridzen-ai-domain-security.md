---
api_specs:
- filename: gridzen-ai-health-api-openapi.yml
  format: yaml
  label: gridzen-ai Health API
  slug: gridzen-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridzen-ai/openapi/gridzen-ai-health-api-openapi.yml
- filename: gridzen-ai-trust-decisions-api-openapi.yml
  format: yaml
  label: gridzen-ai Trust Decisions API
  slug: gridzen-ai-trust-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gridzen-ai/openapi/gridzen-ai-trust-decisions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gridzen.ai
  spf: true
hosts:
- cert_expires: Jan 25 10:24:42 2027 GMT
  host: gridzen.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gridzen Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gridzen-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: gridzen-ai
provider_slug: gridzen-ai
slug: gridzen-ai-domain-security
source_filename: gridzen-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gridzen.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 10:24:42 2027 GMT\n  hsts: false\ndomains:\n- domain: gridzen.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gridzen-ai/security/gridzen-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Energy
- Grid
- Optimization
---
