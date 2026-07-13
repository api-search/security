---
api_specs:
- filename: monnify-authentication-api-openapi.yml
  format: yaml
  label: Monnify Authentication API
  slug: monnify-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-authentication-api-openapi.yml
- filename: monnify-collections-api-openapi.yml
  format: yaml
  label: Monnify Collections API
  slug: monnify-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-collections-api-openapi.yml
- filename: monnify-reserved-accounts-api-openapi.yml
  format: yaml
  label: Monnify Reserved Accounts API
  slug: monnify-reserved-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-reserved-accounts-api-openapi.yml
- filename: monnify-disbursements-api-openapi.yml
  format: yaml
  label: Monnify Disbursements API
  slug: monnify-disbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-disbursements-api-openapi.yml
- filename: monnify-sub-accounts-api-openapi.yml
  format: yaml
  label: Monnify Sub-Accounts API
  slug: monnify-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-sub-accounts-api-openapi.yml
- filename: monnify-direct-debit-api-openapi.yml
  format: yaml
  label: Monnify Direct Debit API
  slug: monnify-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-direct-debit-api-openapi.yml
- filename: monnify-invoices-api-openapi.yml
  format: yaml
  label: Monnify Invoices API
  slug: monnify-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-invoices-api-openapi.yml
- filename: monnify-bills-payment-api-openapi.yml
  format: yaml
  label: Monnify Bills Payment API
  slug: monnify-bills-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-bills-payment-api-openapi.yml
- filename: monnify-verification-api-openapi.yml
  format: yaml
  label: Monnify Verification API
  slug: monnify-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-verification-api-openapi.yml
- filename: monnify-wallets-api-openapi.yml
  format: yaml
  label: Monnify Wallets API
  slug: monnify-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-wallets-api-openapi.yml
- filename: monnify-refunds-api-openapi.yml
  format: yaml
  label: Monnify Refunds API
  slug: monnify-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-refunds-api-openapi.yml
- filename: monnify-settlements-api-openapi.yml
  format: yaml
  label: Monnify Settlements API
  slug: monnify-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-settlements-api-openapi.yml
- filename: moniepoint-pos-api-openapi.yml
  format: yaml
  label: Moniepoint POS Push Payment API
  slug: moniepoint-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-pos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: moniepoint.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: monnify.com
  spf: true
hosts:
- cert_expires: Oct  6 22:17:06 2026 GMT
  host: moniepoint.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 14:19:36 2026 GMT
  host: developers.monnify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 02:49:54 2026 GMT
  host: docs.pos.moniepoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moniepoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moniepoint, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Moniepoint
provider_slug: moniepoint
slug: moniepoint-domain-security
source_filename: moniepoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moniepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:06 2026 GMT\n  hsts: false\n- host: developers.monnify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:19:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pos.moniepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 02:49:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: moniepoint.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: monnify.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/security/moniepoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Africa
- Nigeria
- Payments
- Banking
- Fintech
- Acquiring
- POS
- Collections
- Disbursements
- Virtual Accounts
- Direct Debit
- Bills Payment
- SMB
- Working Capital
- Unicorn
---
