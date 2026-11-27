---
api_specs:
- filename: painspotter-ai-blog-api-openapi.yml
  format: yaml
  label: Pain Spotter Blog API
  slug: painspotter-ai-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/painspotter-ai/openapi/painspotter-ai-blog-api-openapi.yml
- filename: painspotter-ai-opportunities-api-openapi.yml
  format: yaml
  label: Pain Spotter Opportunities API
  slug: painspotter-ai-opportunities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/painspotter-ai/openapi/painspotter-ai-opportunities-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: painspotter.ai
  spf: true
hosts:
- cert_expires: Jan 18 03:45:00 2027 GMT
  host: painspotter.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pain Spotter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pain Spotter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pain Spotter
provider_slug: painspotter-ai
slug: painspotter-ai-domain-security
source_filename: painspotter-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: painspotter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 03:45:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: painspotter.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/painspotter-ai/security/painspotter-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Analytics
- Market Research
- Business Intelligence
- Startup Tools
---
