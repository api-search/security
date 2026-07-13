---
api_specs:
- filename: export-import-bank-of-the-united-states-openapi.yml
  format: yaml
  label: EXIM Open Data API
  slug: open-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/about-exim-exim-gov-export-import-bank-of-the-united-states/refs/heads/main/openapi/export-import-bank-of-the-united-states-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: exim.gov
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: www.exim.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: eximonline.exim.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: data.exim.gov
  https: false
kind: domain-security
layout: security
method: probed
name: Export Import Bank Of The United States Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Export-Import Bank of the United States, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Export-Import Bank of the United States
provider_slug: about-exim-exim-gov-export-import-bank-of-the-united-states
slug: export-import-bank-of-the-united-states-domain-security
source_filename: export-import-bank-of-the-united-states-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exim.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eximonline.exim.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.exim.gov\n  https: false\ndomains:\n- domain: exim.gov\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/about-exim-exim-gov-export-import-bank-of-the-united-states/refs/heads/main/security/export-import-bank-of-the-united-states-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Export
- Federal Government
- Finance
- Import
- Trade Finance
---
