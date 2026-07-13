---
api_specs:
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Charges API
  slug: korapay-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Payouts API
  slug: korapay-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Virtual Bank Accounts API
  slug: korapay-virtual-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Balances API
  slug: korapay-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Refunds API
  slug: korapay-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Currency Conversion API
  slug: korapay-currency-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
- filename: korapay-openapi.yml
  format: yaml
  label: Kora Misc Utilities API
  slug: korapay-misc-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/openapi/korapay-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: korapay.com
  spf: true
  spf_policy: -all
hosts:
- cert_expires: Aug 27 12:38:39 2026 GMT
  host: api.korapay.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:37:59 2026 GMT
  host: korapay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 06:25:34 2026 GMT
  host: korahq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 19:30:48 2026 GMT
  host: developers.korapay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Korapay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kora, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kora
provider_slug: korapay
slug: korapay-domain-security
source_filename: korapay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API hosts\nhosts:\n- host: api.korapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:38:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: korapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:37:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: korahq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:25:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.korapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:30:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: korapay.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_policy: '-all'\n  dmarc: true\n  dmarc_policy: reject\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/korapay/refs/heads/main/security/korapay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Africa
- Nigeria
- Collections
- Payouts
- Disbursements
- Virtual Bank Account
- Cards
- Fintech
---
