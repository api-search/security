---
api_specs:
- filename: emdly-com-openapi-generated.yml
  format: yaml
  label: emdly API
  slug: emdly-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/emdly-com/openapi/_ae-authored/emdly-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: emdly.com
  spf: true
hosts:
- cert_expires: Jan 25 12:28:38 2027 GMT
  host: emdly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: emdly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for emdly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: emdly
provider_slug: emdly-com
slug: emdly-com-domain-security
source_filename: emdly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emdly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 12:28:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: emdly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/emdly-com/security/emdly-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Markdown skills
- Open Source
---
