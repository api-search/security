---
api_specs:
- filename: merqube-api-openapi.json
  format: json
  label: MerQube API
  slug: merqube-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/openapi/merqube-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "ssl.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 issuewild "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: merqube.com
  spf: true
hosts:
- cert_expires: Nov 11 06:18:21 2026 GMT
  host: merqube.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 20:57:01 2026 GMT
  host: www.merqube.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: api.merqube.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Merqube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MerQube, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MerQube
provider_slug: merqube
slug: merqube-domain-security
source_filename: merqube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merqube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 06:18:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: www.merqube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 20:57:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: api.merqube.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: merqube.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/security/merqube-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Financial Services
- Index Data
- Market Data
- Capital Markets
- Investment Strategies
- Asset Management
- ETF
- Structured Products
- Quantitative Finance
- OpenAPI
---
