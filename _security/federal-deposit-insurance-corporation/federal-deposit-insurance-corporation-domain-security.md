---
api_specs:
- filename: federal-deposit-insurance-corporation-demographics-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Demographics API
  slug: federal-deposit-insurance-corporation-demographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-demographics-api-openapi.yml
- filename: federal-deposit-insurance-corporation-deposits-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Deposits API
  slug: federal-deposit-insurance-corporation-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-deposits-api-openapi.yml
- filename: federal-deposit-insurance-corporation-failures-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Failures API
  slug: federal-deposit-insurance-corporation-failures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-failures-api-openapi.yml
- filename: federal-deposit-insurance-corporation-financials-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Financials API
  slug: federal-deposit-insurance-corporation-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-financials-api-openapi.yml
- filename: federal-deposit-insurance-corporation-history-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation History API
  slug: federal-deposit-insurance-corporation-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-history-api-openapi.yml
- filename: federal-deposit-insurance-corporation-institutions-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Institutions API
  slug: federal-deposit-insurance-corporation-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-institutions-api-openapi.yml
- filename: federal-deposit-insurance-corporation-locations-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Locations API
  slug: federal-deposit-insurance-corporation-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-locations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fdic.gov
  spf: true
hosts:
- cert_expires: Aug 17 15:32:11 2026 GMT
  host: www.fdic.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 21:21:32 2026 GMT
  host: banks.data.fdic.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Federal Deposit Insurance Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Deposit Insurance Corporation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Deposit Insurance Corporation
provider_slug: federal-deposit-insurance-corporation
slug: federal-deposit-insurance-corporation-domain-security
source_filename: federal-deposit-insurance-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fdic.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:32:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: banks.data.fdic.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 21:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fdic.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/security/federal-deposit-insurance-corporation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Federal Government
- Financial Data
- Insurance
---
