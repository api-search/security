---
api_specs:
- filename: outworx-openapi-generated.yml
  format: yaml
  label: Outworx API
  slug: outworx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outworx/openapi/_ae-authored/outworx-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: outworx.io
  spf: true
hosts:
- cert_expires: Dec 12 06:12:15 2026 GMT
  host: outworx.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Outworx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outworx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Outworx
provider_slug: outworx
slug: outworx-domain-security
source_filename: outworx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outworx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 06:12:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: outworx.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/outworx/security/outworx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Outsourcing
- B2B SaaS
- Consulting
- Technology
---
