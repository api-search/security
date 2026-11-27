---
api_specs:
- filename: eosl-ai-api-openapi.json
  format: json
  label: EOSL.ai Hardware Lifecycle API API
  slug: eosl-ai-hardware-lifecycle-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eosl-ai/openapi/_original/eosl-ai-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eosl.ai
  spf: true
hosts:
- cert_expires: Jan 15 21:30:12 2027 GMT
  host: eosl.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EOSL.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EOSL.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EOSL.ai
provider_slug: eosl-ai
slug: eosl-ai-domain-security
source_filename: eosl-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eosl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 21:30:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eosl.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/eosl-ai/security/eosl-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Hardware
- Lifecycle
- Data
---
