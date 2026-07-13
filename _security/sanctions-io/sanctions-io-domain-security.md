---
api_specs:
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Screening API
  slug: sanctions-io-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Batch Screening API
  slug: sanctions-io-batch-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Adverse Media API
  slug: sanctions-io-adverse-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Data Sources API
  slug: sanctions-io-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Monitoring API
  slug: sanctions-io-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
- filename: sanctions-io-openapi.yml
  format: yaml
  label: sanctions.io Account Management API
  slug: sanctions-io-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/openapi/sanctions-io-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sanctions.io
  spf: false
hosts:
- cert_expires: Oct  3 05:17:41 2026 GMT
  host: www.sanctions.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 17:51:34 2026 GMT
  host: api-docs.sanctions.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api.sanctions.io
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sanctions Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sanctions.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: sanctions.io
provider_slug: sanctions-io
slug: sanctions-io-domain-security
source_filename: sanctions-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sanctions.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:17:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.sanctions.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 17:51:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sanctions.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: sanctions.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sanctions-io/refs/heads/main/security/sanctions-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Anti-Money Laundering
- AML
- Sanctions Screening
- Compliance
- PEP Screening
- Watchlists
- KYC
- RegTech
---
