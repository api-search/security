---
api_specs:
- filename: immokit-ai-bodenrichtwert-api-openapi.yml
  format: yaml
  label: immokit-ai Bodenrichtwert API
  slug: immokit-ai-bodenrichtwert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immokit-ai/openapi/immokit-ai-bodenrichtwert-api-openapi.yml
- filename: immokit-ai-bodenwert-api-openapi.yml
  format: yaml
  label: immokit-ai Bodenwert API
  slug: immokit-ai-bodenwert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immokit-ai/openapi/immokit-ai-bodenwert-api-openapi.yml
- filename: immokit-ai-me-api-openapi.yml
  format: yaml
  label: immokit-ai Me API
  slug: immokit-ai-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immokit-ai/openapi/immokit-ai-me-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: immokit.ai
  spf: true
hosts:
- cert_expires: Dec 24 12:28:38 2026 GMT
  host: immokit.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: immokit-ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for immokit-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: immokit-ai
provider_slug: immokit-ai
slug: immokit-ai-domain-security
source_filename: immokit-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: immokit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 12:28:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: immokit.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/immokit-ai/security/immokit-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
