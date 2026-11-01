---
api_specs:
- filename: green-api-com-openapi-generated.yml
  format: yaml
  label: green-api-com API
  slug: green-api-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/green-api-com/openapi/_ae-authored/green-api-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: green-api.com
  spf: true
hosts:
- cert_expires: Jan 10 05:14:17 2027 GMT
  host: green-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Green Api Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for green-api-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: green-api-com
provider_slug: green-api-com
slug: green-api-com-domain-security
source_filename: green-api-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: green-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 05:14:17 2027 GMT\n  hsts: false\ndomains:\n- domain: green-api.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/green-api-com/security/green-api-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Messaging
- WhatsApp
- API
- Integration
---
