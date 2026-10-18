---
api_specs:
- filename: mocki-openapi-generated.yml
  format: yaml
  label: Mocki API
  slug: mocki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mocki/refs/heads/main/openapi/_ae-authored/mocki-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mocki.io
  spf: false
hosts:
- cert_expires: Apr  6 23:59:59 2027 GMT
  host: mocki.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mocki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mocki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mocki
provider_slug: mocki
slug: mocki-domain-security
source_filename: mocki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mocki.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: mocki.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mocki/refs/heads/main/security/mocki-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- SaaS
- Mock API
- Testing
- Development
---
