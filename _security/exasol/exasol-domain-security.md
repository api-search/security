---
api_specs:
- filename: exasol-openapi-generated.yml
  format: yaml
  label: Exasol API
  slug: exasol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/exasol/openapi/_ae-authored/exasol-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "thawte.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "certainly.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: exasol.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: exasol.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Exasol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exasol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Exasol
provider_slug: exasol
slug: exasol-domain-security
source_filename: exasol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: exasol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: exasol.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"thawte.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/exasol/security/exasol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Database
- Analytics
- Artificial Intelligence
- Data Warehouse
---
