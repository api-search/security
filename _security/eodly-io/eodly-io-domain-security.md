---
api_specs:
- filename: eodly-io-api-openapi.json
  format: json
  label: Eodly API API
  slug: eodly-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eodly-io/openapi/_original/eodly-io-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eodly.io
  spf: true
hosts:
- cert_expires: Jan 14 05:13:46 2027 GMT
  host: eodly.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eodly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eodly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eodly
provider_slug: eodly-io
slug: eodly-io-domain-security
source_filename: eodly-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eodly.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 05:13:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eodly.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eodly-io/security/eodly-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Productivity
- Remote Work
- Team Management
- Reporting
---
