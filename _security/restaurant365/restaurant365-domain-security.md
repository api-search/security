---
api_specs:
- filename: restaurant365-ap-invoices-api-openapi.yml
  format: yaml
  label: Restaurant365 AP Invoices API
  slug: restaurant365-ap-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-ap-invoices-api-openapi.yml
- filename: restaurant365-audit-api-openapi.yml
  format: yaml
  label: Restaurant365 Audit API
  slug: restaurant365-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-audit-api-openapi.yml
- filename: restaurant365-authentication-api-openapi.yml
  format: yaml
  label: Restaurant365 Authentication API
  slug: restaurant365-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-authentication-api-openapi.yml
- filename: restaurant365-general-ledger-api-openapi.yml
  format: yaml
  label: Restaurant365 General Ledger API
  slug: restaurant365-general-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-general-ledger-api-openapi.yml
- filename: restaurant365-labor-api-openapi.yml
  format: yaml
  label: Restaurant365 Labor API
  slug: restaurant365-labor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-labor-api-openapi.yml
- filename: restaurant365-metadata-api-openapi.yml
  format: yaml
  label: Restaurant365 Metadata API
  slug: restaurant365-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-metadata-api-openapi.yml
- filename: restaurant365-reference-data-api-openapi.yml
  format: yaml
  label: Restaurant365 Reference Data API
  slug: restaurant365-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-reference-data-api-openapi.yml
- filename: restaurant365-sales-api-openapi.yml
  format: yaml
  label: Restaurant365 Sales API
  slug: restaurant365-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-sales-api-openapi.yml
- filename: restaurant365-transactions-api-openapi.yml
  format: yaml
  label: Restaurant365 Transactions API
  slug: restaurant365-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/openapi/restaurant365-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: restaurant365.com
  spf: true
hosts:
- cert_expires: Sep 30 06:44:34 2026 GMT
  host: www.restaurant365.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 16:42:21 2026 GMT
  host: docs.restaurant365.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 14:07:42 2027 GMT
  host: yourcompany.restaurant365.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Restaurant365 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Restaurant365, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Restaurant365
provider_slug: restaurant365
slug: restaurant365-domain-security
source_filename: restaurant365-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.restaurant365.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:44:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.restaurant365.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 16:42:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yourcompany.restaurant365.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 11 14:07:42 2027 GMT\n  hsts: false\ndomains:\n- domain: restaurant365.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restaurant365/refs/heads/main/security/restaurant365-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Accounting
- Inventory
- Invoices
- Reporting
- OData
---
