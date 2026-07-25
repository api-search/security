---
api_specs:
- filename: finicity-openbanking-us-openapi-original.yml
  format: yaml
  label: Finicity Aggregation (Accounts & Transactions) API
  slug: finicity-aggregation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finicity/refs/heads/main/openapi/finicity-openbanking-us-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: finicity.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mastercard.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.finicity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: developer.mastercard.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.finicity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finicity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finicity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Finicity
provider_slug: finicity
slug: finicity-domain-security
source_filename: finicity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.finicity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\n- host: developer.mastercard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: api.finicity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: finicity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mastercard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finicity/refs/heads/main/security/finicity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Data Aggregation
- Open Finance
- Open Banking
- FDX
- United States
- Payments
- Financial Data
---
