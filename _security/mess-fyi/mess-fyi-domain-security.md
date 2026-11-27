---
api_specs:
- filename: mess-fyi-openapi-generated.yml
  format: yaml
  label: MESS API
  slug: mess-fyi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mess-fyi/openapi/_ae-authored/mess-fyi-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mess.fyi
  spf: true
hosts:
- cert_expires: Dec 31 03:37:38 2026 GMT
  host: mess.fyi
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MESS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MESS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MESS
provider_slug: mess-fyi
slug: mess-fyi-domain-security
source_filename: mess-fyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mess.fyi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 03:37:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mess.fyi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mess-fyi/security/mess-fyi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Service Accounts
- Ledger
- Monitoring
- Open Source
---
