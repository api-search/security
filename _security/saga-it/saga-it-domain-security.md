---
api_specs:
- filename: saga-it-openapi-generated.yml
  format: yaml
  label: Saga IT API
  slug: saga-it-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/saga-it/openapi/_ae-authored/saga-it-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saga-it.com
  spf: true
hosts:
- cert_expires: Dec 23 19:46:52 2026 GMT
  host: saga-it.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Saga It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saga IT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Saga IT
provider_slug: saga-it
slug: saga-it-domain-security
source_filename: saga-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saga-it.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 19:46:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: saga-it.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/saga-it/security/saga-it-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- IT Consulting
- Interoperability
- Cloud Services
---
