---
api_specs:
- filename: cuein-insights-openapi.json
  format: json
  label: Cuein Insights API
  slug: cuein-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuein/refs/heads/main/openapi/cuein-insights-openapi.json
- filename: cuein-answers-openapi.json
  format: json
  label: Cuein Answers API
  slug: cuein-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuein/refs/heads/main/openapi/cuein-answers-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cuein.ai
  spf: false
hosts:
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: cuein-api.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.cuein.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Cuein Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cuein, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cuein
provider_slug: cuein
slug: cuein-domain-security
source_filename: cuein-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cuein-api.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cuein.ai\n  https: false\ndomains:\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cuein.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuein/refs/heads/main/security/cuein-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Experience
- Customer Support
- Conversation Intelligence
- Generative AI
- Insights
- Knowledge Base
- Contact Center
---
