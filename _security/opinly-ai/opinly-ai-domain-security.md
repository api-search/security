---
api_specs:
- filename: opinly-ai-content-api-openapi.yml
  format: yaml
  label: Opinly Content API
  slug: opinly-ai-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opinly-ai/openapi/opinly-ai-content-api-openapi.yml
- filename: opinly-ai-events-api-openapi.yml
  format: yaml
  label: Opinly Events API
  slug: opinly-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opinly-ai/openapi/opinly-ai-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: opinly.ai
  spf: true
hosts:
- cert_expires: Apr  6 23:59:59 2027 GMT
  host: opinly.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opinly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opinly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Opinly
provider_slug: opinly-ai
slug: opinly-ai-domain-security
source_filename: opinly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opinly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opinly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/opinly-ai/security/opinly-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SEO
- Artificial Intelligence
- Marketing
- Automation
---
