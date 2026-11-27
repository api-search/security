---
api_specs:
- filename: launch529-com-openapi-generated.yml
  format: yaml
  label: Launch529 API
  slug: launch529-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/launch529-com/openapi/_ae-authored/launch529-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: launch529.com
  spf: true
hosts:
- cert_expires: Dec 31 00:37:02 2026 GMT
  host: launch529.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Launch529 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Launch529, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Launch529
provider_slug: launch529-com
slug: launch529-com-domain-security
source_filename: launch529-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: launch529.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 00:37:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: launch529.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/launch529-com/security/launch529-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- 529 Savings
- College Savings Planner
- Expense Tracking
- IRS Compliance
---
