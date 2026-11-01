---
api_specs:
- filename: pianam-cn-default-api-openapi.yml
  format: yaml
  label: Mycel AI
  slug: mycel-ai
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pianam-cn/openapi/pianam-cn-default-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pianam.cn
  spf: false
hosts:
- cert_expires: Jan 11 08:39:57 2027 GMT
  host: pianam.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pianam Cn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pianam-cn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: pianam-cn
provider_slug: pianam-cn
slug: pianam-cn-domain-security
source_filename: pianam-cn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pianam.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 08:39:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pianam.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pianam-cn/security/pianam-cn-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Chatbot
- Conversation
- Chinese
---
