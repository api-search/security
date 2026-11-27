---
api_specs:
- filename: graphify-com-openapi-generated.yml
  format: yaml
  label: Graphify API
  slug: graphify-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/graphify-com/openapi/_ae-authored/graphify-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: graphify.com
  spf: true
hosts:
- cert_expires: Feb  8 01:31:57 2027 GMT
  host: graphify.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Graphify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graphify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Graphify
provider_slug: graphify-com
slug: graphify-com-domain-security
source_filename: graphify-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graphify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 01:31:57 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: graphify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/graphify-com/security/graphify-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- code graph
- Developer Tools
- Source Code Analysis
- Pull Request Review
- Open Source
- Hosted Service
---
