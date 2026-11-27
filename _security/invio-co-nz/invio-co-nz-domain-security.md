---
api_specs:
- filename: invio-co-nz-openapi-generated.yml
  format: yaml
  label: Invio API
  slug: invio-co-nz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invio-co-nz/openapi/_ae-authored/invio-co-nz-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: invio.co.nz
  spf: true
hosts:
- cert_expires: Jan 12 13:56:29 2027 GMT
  host: invio.co.nz
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Invio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Invio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Invio
provider_slug: invio-co-nz
slug: invio-co-nz-domain-security
source_filename: invio-co-nz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: invio.co.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 13:56:29 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: invio.co.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/invio-co-nz/security/invio-co-nz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Invoicing
- NZ
- Software-as-a-Service
- Small Business
- Fintech
---
