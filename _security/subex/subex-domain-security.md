---
api_specs:
- filename: subex-analytics-api-openapi.yml
  format: yaml
  label: Subex Analytics API
  slug: subex-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subex/refs/heads/main/openapi/subex-analytics-api-openapi.yml
- filename: subex-fraud-management-api-openapi.yml
  format: yaml
  label: Subex Fraud Management API
  slug: subex-fraud-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subex/refs/heads/main/openapi/subex-fraud-management-api-openapi.yml
- filename: subex-reconciliation-api-openapi.yml
  format: yaml
  label: Subex Reconciliation API
  slug: subex-reconciliation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subex/refs/heads/main/openapi/subex-reconciliation-api-openapi.yml
- filename: subex-revenue-assurance-api-openapi.yml
  format: yaml
  label: Subex Revenue Assurance API
  slug: subex-revenue-assurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subex/refs/heads/main/openapi/subex-revenue-assurance-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: subex.com
  spf: true
hosts:
- cert_expires: Sep 17 01:39:05 2026 GMT
  host: www.subex.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Subex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Subex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Subex
provider_slug: subex
slug: subex-domain-security
source_filename: subex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.subex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:39:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: subex.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subex/refs/heads/main/security/subex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Telecom
- Revenue Assurance
- Fraud Management
- Analytics
- BSS/OSS
---
