---
api_specs:
- filename: kourier-sh-feedback-api-openapi.yml
  format: yaml
  label: Kourier Feedback API
  slug: kourier-sh-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kourier-sh/openapi/kourier-sh-feedback-api-openapi.yml
- filename: kourier-sh-chat-completions-api-openapi.yml
  format: yaml
  label: Kourier Chat Completions API
  slug: kourier-sh-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kourier-sh/openapi/kourier-sh-chat-completions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: kourier.sh
  spf: true
hosts:
- cert_expires: Jan  1 05:38:29 2027 GMT
  host: kourier.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kourier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kourier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Kourier
provider_slug: kourier-sh
slug: kourier-sh-domain-security
source_filename: kourier-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kourier.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 05:38:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kourier.sh\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kourier-sh/security/kourier-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Inference
- OpenAI-Compatible
- Flat-rate
- Coding Agents
- Models
---
