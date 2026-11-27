---
api_specs:
- filename: maxcv-ai-account-api-openapi.yml
  format: yaml
  label: MaxCV Account API
  slug: maxcv-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-account-api-openapi.yml
- filename: maxcv-ai-cv-api-openapi.yml
  format: yaml
  label: MaxCV Cv API
  slug: maxcv-ai-cv-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-cv-api-openapi.yml
- filename: maxcv-ai-matches-api-openapi.yml
  format: yaml
  label: MaxCV Matches API
  slug: maxcv-ai-matches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-matches-api-openapi.yml
- filename: maxcv-ai-render-api-openapi.yml
  format: yaml
  label: MaxCV Render API
  slug: maxcv-ai-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-render-api-openapi.yml
- filename: maxcv-ai-score-api-openapi.yml
  format: yaml
  label: MaxCV Score API
  slug: maxcv-ai-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-score-api-openapi.yml
- filename: maxcv-ai-tailor-api-openapi.yml
  format: yaml
  label: MaxCV Tailor API
  slug: maxcv-ai-tailor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxcv-ai/openapi/maxcv-ai-tailor-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: maxcv.ai
  spf: true
hosts:
- cert_expires: Jan  5 03:25:17 2027 GMT
  host: maxcv.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MaxCV Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MaxCV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MaxCV
provider_slug: maxcv-ai
slug: maxcv-ai-domain-security
source_filename: maxcv-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maxcv.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 03:25:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maxcv.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/maxcv-ai/security/maxcv-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Resume
- Job Search
- Careers
- Automation
- Company
---
