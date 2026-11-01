---
api_specs:
- filename: open-banking-openapi-generated.yml
  format: yaml
  label: Tatic API
  slug: open-banking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/open-banking/openapi/_ae-authored/open-banking-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: open-banking.io
  spf: true
hosts:
- cert_expires: Jan  3 13:58:15 2027 GMT
  host: open-banking.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Banking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tatic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tatic
provider_slug: open-banking
slug: open-banking-domain-security
source_filename: open-banking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open-banking.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 13:58:15 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: open-banking.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/open-banking/security/open-banking-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
