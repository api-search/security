---
api_specs:
- filename: pepbank-io-account-api-openapi.yml
  format: yaml
  label: PepBank Account API
  slug: pepbank-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pepbank-io/openapi/pepbank-io-account-api-openapi.yml
- filename: pepbank-io-contribute-api-openapi.yml
  format: yaml
  label: PepBank Contribute API
  slug: pepbank-io-contribute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pepbank-io/openapi/pepbank-io-contribute-api-openapi.yml
- filename: pepbank-io-evidence-api-openapi.yml
  format: yaml
  label: PepBank Evidence API
  slug: pepbank-io-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pepbank-io/openapi/pepbank-io-evidence-api-openapi.yml
- filename: pepbank-io-exports-api-openapi.yml
  format: yaml
  label: PepBank Exports API
  slug: pepbank-io-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pepbank-io/openapi/pepbank-io-exports-api-openapi.yml
- filename: pepbank-io-peptides-api-openapi.yml
  format: yaml
  label: PepBank Peptides API
  slug: pepbank-io-peptides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pepbank-io/openapi/pepbank-io-peptides-api-openapi.yml
- filename: pepbank-io-records-api-openapi.yml
  format: yaml
  label: PepBank Records API
  slug: pepbank-io-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pepbank-io/openapi/pepbank-io-records-api-openapi.yml
- filename: pepbank-io-sync-api-openapi.yml
  format: yaml
  label: PepBank Sync API
  slug: pepbank-io-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pepbank-io/openapi/pepbank-io-sync-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pepbank.io
  spf: true
hosts:
- cert_expires: Jan 19 19:46:53 2027 GMT
  host: pepbank.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: PepBank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PepBank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PepBank
provider_slug: pepbank-io
slug: pepbank-io-domain-security
source_filename: pepbank-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pepbank.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 19:46:53 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pepbank.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pepbank-io/security/pepbank-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Peptides
- Research
- Database
- Biotechnology
- Free
---
