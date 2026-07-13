---
api_specs:
- filename: ncua-credit-union-locator-api-openapi.yml
  format: yaml
  label: NCUA Credit Union Locator API
  slug: credit-union-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncua/refs/heads/main/openapi/ncua-credit-union-locator-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ncua.gov
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: ncua.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: mapping.ncua.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.ncua.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ncua Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Credit Union Administration (NCUA), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Credit Union Administration (NCUA)
provider_slug: ncua
slug: ncua-domain-security
source_filename: ncua-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ncua.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mapping.ncua.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ncua.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ncua.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ncua/refs/heads/main/security/ncua-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Credit Unions
- Financial Data
- Call Reports
- Banking
- Regulatory Data
---
