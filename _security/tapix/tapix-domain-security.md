---
api_specs:
- filename: tapix-openapi-generated.yml
  format: yaml
  label: Dateio API
  slug: tapix-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tapix/openapi/_ae-authored/tapix-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tapix.io
  spf: true
hosts:
- cert_expires: Nov 28 03:10:51 2026 GMT
  host: tapix.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tapix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dateio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dateio
provider_slug: tapix
slug: tapix-domain-security
source_filename: tapix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tapix.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 03:10:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tapix.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tapix/security/tapix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Data Enrichment
---
