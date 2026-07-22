---
api_specs:
- filename: recurrency-openapi.yml
  format: yaml
  label: Recurrency API
  slug: recurrency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recurrency/refs/heads/main/openapi/recurrency-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: recurrency.com
  spf: true
hosts:
- cert_expires: Oct 11 21:12:51 2026 GMT
  host: www.recurrency.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: api.recurrency.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: api-staging.recurrency.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Recurrency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recurrency, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Recurrency
provider_slug: recurrency
slug: recurrency-domain-security
source_filename: recurrency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.recurrency.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 21:12:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.recurrency.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\n- host: api-staging.recurrency.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: recurrency.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recurrency/refs/heads/main/security/recurrency-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- ERP
- Distribution
- Wholesale
- E-Procurement
- Supply Chain
- Orders
---
