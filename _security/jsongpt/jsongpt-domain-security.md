---
api_specs:
- filename: jsongpt-api-openapi.yml
  format: yaml
  label: JSON GPT API API
  slug: json-gpt-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jsongpt/refs/heads/main/openapi/_original/jsongpt-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jsongpt.com
  spf: true
hosts:
- cert_expires: Dec 21 12:35:05 2026 GMT
  host: jsongpt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jsongpt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JsonGPT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: JsonGPT
provider_slug: jsongpt
slug: jsongpt-domain-security
source_filename: jsongpt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jsongpt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 12:35:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jsongpt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jsongpt/refs/heads/main/security/jsongpt-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- JSON
- API
- Automation
---
