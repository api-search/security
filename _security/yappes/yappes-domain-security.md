---
api_specs:
- filename: yappes-openapi-generated.yml
  format: yaml
  label: Yappes API
  slug: yappes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappes/openapi/_ae-authored/yappes-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yappes.com
  spf: true
hosts:
- cert_expires: Dec 22 22:13:51 2026 GMT
  host: yappes.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yappes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yappes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yappes
provider_slug: yappes
slug: yappes-domain-security
source_filename: yappes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yappes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 22:13:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yappes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/yappes/security/yappes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API Management
- Unified Platform
- Developer Portal
- Analytics
---
