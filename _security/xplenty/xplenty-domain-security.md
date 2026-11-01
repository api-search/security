---
api_specs:
- filename: xplenty-openapi-generated.yml
  format: yaml
  label: Integrate.io API
  slug: xplenty-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xplenty/openapi/_ae-authored/xplenty-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "starfieldtech.com"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xplenty.com
  spf: true
hosts:
- cert_expires: Dec  4 02:40:02 2026 GMT
  host: xplenty.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xplenty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Integrate.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Integrate.io
provider_slug: xplenty
slug: xplenty-domain-security
source_filename: xplenty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xplenty.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 02:40:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xplenty.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/xplenty/security/xplenty-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Data Integration
- ETL
- Low-Code
- Artificial Intelligence
- Cloud
---
