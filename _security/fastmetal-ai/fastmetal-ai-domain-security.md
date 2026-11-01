---
api_specs:
- filename: fastmetal-ai-api-openapi-generated.yml
  format: yaml
  label: fastmetal-ai api API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastmetal-ai/openapi/_ae-authored/fastmetal-ai-api-openapi-generated.yml
- filename: fastmetal-ai-core-openapi-generated.yml
  format: yaml
  label: fastmetal-ai core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastmetal-ai/openapi/_ae-authored/fastmetal-ai-core-openapi-generated.yml
- filename: fastmetal-ai-guides-openapi-generated.yml
  format: yaml
  label: fastmetal-ai All guides API
  slug: guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastmetal-ai/openapi/_ae-authored/fastmetal-ai-guides-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fastmetal.ai
  spf: true
hosts:
- cert_expires: Jan 11 06:02:24 2027 GMT
  host: fastmetal.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fastmetal Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fastmetal-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: fastmetal-ai
provider_slug: fastmetal-ai
slug: fastmetal-ai-domain-security
source_filename: fastmetal-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fastmetal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 06:02:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fastmetal.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fastmetal-ai/security/fastmetal-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- API
- Platform
- Cloud
---
