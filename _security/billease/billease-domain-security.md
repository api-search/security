---
api_specs:
- filename: billease-be-store-admin-api-api-openapi.yml
  format: yaml
  label: Billease Be Store Admin API
  slug: billease-be-store-admin-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billease/refs/heads/main/openapi/billease-be-store-admin-api-api-openapi.yml
- filename: billease-be-transactions-api-api-openapi.yml
  format: yaml
  label: Billease Be Transactions API
  slug: billease-be-transactions-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billease/refs/heads/main/openapi/billease-be-transactions-api-api-openapi.yml
- filename: billease-categories-api-openapi.yml
  format: yaml
  label: Billease Categories API
  slug: billease-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billease/refs/heads/main/openapi/billease-categories-api-openapi.yml
- filename: billease-products-api-openapi.yml
  format: yaml
  label: Billease Products API
  slug: billease-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billease/refs/heads/main/openapi/billease-products-api-openapi.yml
- filename: billease-trx-api-openapi.yml
  format: yaml
  label: Billease Trx API
  slug: billease-trx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/billease/refs/heads/main/openapi/billease-trx-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: billease.ph
  spf: true
hosts:
- cert_expires: Dec 16 00:06:04 2026 GMT
  host: billease.ph
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Billease Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Billease, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Billease
provider_slug: billease
slug: billease-domain-security
source_filename: billease-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: billease.ph\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 00:06:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: billease.ph\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billease/refs/heads/main/security/billease-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Buy Now Pay Later
- Philippines
- Loans
---
