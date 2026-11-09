---
api_specs:
- filename: arpi-ai-authentication-api-openapi.yml
  format: yaml
  label: ARPI Inc. Authentication API
  slug: arpi-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arpi-ai/openapi/arpi-ai-authentication-api-openapi.yml
- filename: arpi-ai-diag-api-openapi.yml
  format: yaml
  label: ARPI Inc. Diag API
  slug: arpi-ai-diag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arpi-ai/openapi/arpi-ai-diag-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: arpi.ai
  spf: true
hosts:
- cert_expires: Dec  8 03:40:16 2026 GMT
  host: arpi.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arpi Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ARPI Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ARPI Inc.
provider_slug: arpi-ai
slug: arpi-ai-domain-security
source_filename: arpi-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arpi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 03:40:16 2026 GMT\n  hsts: false\ndomains:\n- domain: arpi.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/arpi-ai/security/arpi-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Medical AI
- Healthcare
- ECG
- Diagnostics
- Artificial Intelligence
---
