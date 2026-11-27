---
api_specs:
- filename: arvx-ai-readings-api-openapi.yml
  format: yaml
  label: ARVX Readings API
  slug: arvx-ai-readings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arvx-ai/openapi/arvx-ai-readings-api-openapi.yml
- filename: arvx-ai-records-api-openapi.yml
  format: yaml
  label: ARVX Records API
  slug: arvx-ai-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arvx-ai/openapi/arvx-ai-records-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arvx.ai
  spf: true
hosts:
- cert_expires: Jan 28 02:01:03 2027 GMT
  host: arvx.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ARVX Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ARVX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ARVX
provider_slug: arvx-ai
slug: arvx-ai-domain-security
source_filename: arvx-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arvx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 02:01:03 2027 GMT\n  hsts: false\ndomains:\n- domain: arvx.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/arvx-ai/security/arvx-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
