---
api_specs:
- filename: numberrank-dev-badge-api-openapi.yml
  format: yaml
  label: numberRank Badge API
  slug: numberrank-dev-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numberrank-dev/openapi/numberrank-dev-badge-api-openapi.yml
- filename: numberrank-dev-check-api-openapi.yml
  format: yaml
  label: numberRank Check API
  slug: numberrank-dev-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numberrank-dev/openapi/numberrank-dev-check-api-openapi.yml
- filename: numberrank-dev-directory-api-openapi.yml
  format: yaml
  label: numberRank Directory API
  slug: numberrank-dev-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numberrank-dev/openapi/numberrank-dev-directory-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: numberrank.dev
  spf: false
hosts:
- cert_expires: Feb 15 20:42:16 2027 GMT
  host: numberrank.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: numberRank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for numberRank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: numberRank
provider_slug: numberrank-dev
slug: numberrank-dev-domain-security
source_filename: numberrank-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numberrank.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 20:42:16 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: numberrank.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/numberrank-dev/security/numberrank-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Phone
- Fraud Prevention
- VoIP Detection
---
