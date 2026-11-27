---
api_specs:
- filename: echoai-so-openapi-generated.yml
  format: yaml
  label: Echo AI API
  slug: echoai-so-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/echoai-so/openapi/_ae-authored/echoai-so-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: echoai.so
  spf: true
hosts:
- cert_expires: Jan 21 21:50:12 2027 GMT
  host: echoai.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Echo AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Echo AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Echo AI
provider_slug: echoai-so
slug: echoai-so-domain-security
source_filename: echoai-so-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: echoai.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 21:50:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: echoai.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/echoai-so/security/echoai-so-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Software-as-a-Service
- Chatbots
- No-Code
- Multi-Channel
---
