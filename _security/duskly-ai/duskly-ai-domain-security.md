---
api_specs:
- filename: duskly-ai-health-api-openapi.yml
  format: yaml
  label: duskly-ai Health API
  slug: duskly-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duskly-ai/openapi/duskly-ai-health-api-openapi.yml
- filename: duskly-ai-verify-api-openapi.yml
  format: yaml
  label: duskly-ai Verify API
  slug: duskly-ai-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duskly-ai/openapi/duskly-ai-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: duskly.ai
  spf: true
hosts:
- cert_expires: Jan 31 20:36:46 2027 GMT
  host: duskly.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: duskly-ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for duskly-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: duskly-ai
provider_slug: duskly-ai
slug: duskly-ai-domain-security
source_filename: duskly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: duskly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 20:36:46 2027 GMT\n  hsts: false\ndomains:\n- domain: duskly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/duskly-ai/security/duskly-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Virtual Staging
- AI Photo Editing
- Real Estate
- MLS Compliance
- Real Estate Tools
---
