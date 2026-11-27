---
api_specs:
- filename: electrik-dev-openapi-generated.yml
  format: yaml
  label: Electrik API
  slug: electrik-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/electrik-dev/openapi/_ae-authored/electrik-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: electrik.dev
  spf: true
hosts:
- cert_expires: Dec 24 22:57:16 2026 GMT
  host: electrik.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Electrik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electrik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Electrik
provider_slug: electrik-dev
slug: electrik-dev-domain-security
source_filename: electrik-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: electrik.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 22:57:16 2026 GMT\n  hsts: false\ndomains:\n- domain: electrik.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/electrik-dev/security/electrik-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Laravel
- Software-as-a-Service
- Stripe
- Open Source
- PHP
---
