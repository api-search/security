---
api_specs:
- filename: treasury-fiscal-data-api-openapi.yaml
  format: yaml
  label: Treasury Fiscal Data API
  slug: fiscal-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/u-s-treasury-fiscal-data/refs/heads/main/openapi/treasury-fiscal-data-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: treasury.gov
  spf: true
hosts:
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: fiscaldata.treasury.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: api.fiscaldata.treasury.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: U S Treasury Fiscal Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for U.S. Treasury Fiscal Data, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: U.S. Treasury Fiscal Data
provider_slug: u-s-treasury-fiscal-data
slug: u-s-treasury-fiscal-data-domain-security
source_filename: u-s-treasury-fiscal-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fiscaldata.treasury.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fiscaldata.treasury.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: treasury.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/u-s-treasury-fiscal-data/refs/heads/main/security/u-s-treasury-fiscal-data-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Finance
- Treasury
- National Debt
- Exchange Rates
- Economics
---
