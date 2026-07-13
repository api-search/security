---
api_specs:
- filename: tiaa-fdx-openapi.yml
  format: yaml
  label: TIAA Financial Data Exchange API
  slug: tiaa-fdx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-fdx-openapi.yml
- filename: tiaa-sia-openapi.yml
  format: yaml
  label: TIAA Secure Income Account API
  slug: tiaa-sia-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/openapi/tiaa-sia-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tiaa.org
  spf: true
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: developer.tiaa.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: www.tiaa.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.tiaa.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tiaa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TIAA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TIAA
provider_slug: tiaa
slug: tiaa-domain-security
source_filename: tiaa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.tiaa.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\n- host: www.tiaa.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: null\n- host: api.tiaa.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tiaa.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiaa/refs/heads/main/security/tiaa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Financial Data
- Fintech
- Insurance
- Investment Management
- Retirement
- Wealth Management
- Fortune 100
---
