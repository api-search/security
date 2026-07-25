---
api_specs:
- filename: procurify-account-codes-api-openapi.yml
  format: yaml
  label: Procurify account-codes API
  slug: procurify-account-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-account-codes-api-openapi.yml
- filename: procurify-accounts-api-openapi.yml
  format: yaml
  label: Procurify accounts API
  slug: procurify-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-accounts-api-openapi.yml
- filename: procurify-ap-api-openapi.yml
  format: yaml
  label: Procurify ap API
  slug: procurify-ap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-ap-api-openapi.yml
- filename: procurify-catalog-api-openapi.yml
  format: yaml
  label: Procurify catalog API
  slug: procurify-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-catalog-api-openapi.yml
- filename: procurify-currencies-api-openapi.yml
  format: yaml
  label: Procurify currencies API
  slug: procurify-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-currencies-api-openapi.yml
- filename: procurify-custom-fields-api-openapi.yml
  format: yaml
  label: Procurify custom-fields API
  slug: procurify-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-custom-fields-api-openapi.yml
- filename: procurify-departments-api-openapi.yml
  format: yaml
  label: Procurify departments API
  slug: procurify-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-departments-api-openapi.yml
- filename: procurify-locations-api-openapi.yml
  format: yaml
  label: Procurify locations API
  slug: procurify-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-locations-api-openapi.yml
- filename: procurify-oauth-api-openapi.yml
  format: yaml
  label: Procurify oauth API
  slug: procurify-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-oauth-api-openapi.yml
- filename: procurify-order-items-api-openapi.yml
  format: yaml
  label: Procurify order-items API
  slug: procurify-order-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-order-items-api-openapi.yml
- filename: procurify-permissions-api-openapi.yml
  format: yaml
  label: Procurify permissions API
  slug: procurify-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-permissions-api-openapi.yml
- filename: procurify-public-api-openapi.yml
  format: yaml
  label: Procurify public API
  slug: procurify-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-public-api-openapi.yml
- filename: procurify-purchase-orders-api-openapi.yml
  format: yaml
  label: Procurify purchase-orders API
  slug: procurify-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-purchase-orders-api-openapi.yml
- filename: procurify-receipt-api-openapi.yml
  format: yaml
  label: Procurify receipt API
  slug: procurify-receipt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-receipt-api-openapi.yml
- filename: procurify-requisitions-api-openapi.yml
  format: yaml
  label: Procurify requisitions API
  slug: procurify-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-requisitions-api-openapi.yml
- filename: procurify-users-api-openapi.yml
  format: yaml
  label: Procurify users API
  slug: procurify-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-users-api-openapi.yml
- filename: procurify-vendors-api-openapi.yml
  format: yaml
  label: Procurify vendors API
  slug: procurify-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/openapi/procurify-vendors-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: procurify.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.procurify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 07:17:13 2026 GMT
  host: developer.procurify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.procurify.com
  https: false
kind: domain-security
layout: security
method: probed
name: Procurify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Procurify, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Procurify
provider_slug: procurify
slug: procurify-domain-security
source_filename: procurify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.procurify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\n- host: developer.procurify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:17:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.procurify.com\n  https: false\ndomains:\n- domain: procurify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/security/procurify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Spend Management
- Procurement
- Purchase Orders
- Accounts Payable
- Vendor Management
- Budget Tracking
- Procure-to-Pay
- ERP Integration
---
