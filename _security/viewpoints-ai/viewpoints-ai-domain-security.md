---
api_specs:
- filename: viewpoints-ai-study-openapi.json
  format: json
  label: Viewpoints Study API
  slug: viewpoints-study-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viewpoints-ai/refs/heads/main/openapi/viewpoints-ai-study-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: viewpoints.ai
  spf: true
hosts:
- cert_expires: Sep 19 18:08:43 2026 GMT
  host: viewpoints.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Viewpoints Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Viewpoints AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Viewpoints AI
provider_slug: viewpoints-ai
slug: viewpoints-ai-domain-security
source_filename: viewpoints-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: viewpoints.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 18:08:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: viewpoints.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viewpoints-ai/refs/heads/main/security/viewpoints-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Market Research
- Synthetic Personas
- Consumer Insights
- Litigation
- Jury Simulation
- Research
---
