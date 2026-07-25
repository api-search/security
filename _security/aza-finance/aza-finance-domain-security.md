---
api_specs:
- filename: aza-finance-account-debits-api-openapi.yml
  format: yaml
  label: AZA Finance Account Debits API
  slug: aza-finance-account-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-account-debits-api-openapi.yml
- filename: aza-finance-account-validation-api-openapi.yml
  format: yaml
  label: AZA Finance Account Validation API
  slug: aza-finance-account-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-account-validation-api-openapi.yml
- filename: aza-finance-accounts-api-openapi.yml
  format: yaml
  label: AZA Finance Accounts API
  slug: aza-finance-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-accounts-api-openapi.yml
- filename: aza-finance-api-logs-api-openapi.yml
  format: yaml
  label: AZA Finance API Logs API
  slug: aza-finance-api-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-api-logs-api-openapi.yml
- filename: aza-finance-currency-info-api-openapi.yml
  format: yaml
  label: AZA Finance Currency Info API
  slug: aza-finance-currency-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-currency-info-api-openapi.yml
- filename: aza-finance-dlocal-balance-api-openapi.yml
  format: yaml
  label: AZA Finance dlocal balance API
  slug: aza-finance-dlocal-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-dlocal-balance-api-openapi.yml
- filename: aza-finance-documents-api-openapi.yml
  format: yaml
  label: AZA Finance Documents API
  slug: aza-finance-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-documents-api-openapi.yml
- filename: aza-finance-logs-api-openapi.yml
  format: yaml
  label: AZA Finance Logs API
  slug: aza-finance-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-logs-api-openapi.yml
- filename: aza-finance-mandates-api-openapi.yml
  format: yaml
  label: AZA Finance Mandates API
  slug: aza-finance-mandates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-mandates-api-openapi.yml
- filename: aza-finance-payin-methods-api-openapi.yml
  format: yaml
  label: AZA Finance Payin Methods API
  slug: aza-finance-payin-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-payin-methods-api-openapi.yml
- filename: aza-finance-payment-methods-api-openapi.yml
  format: yaml
  label: AZA Finance Payment Methods API
  slug: aza-finance-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-payment-methods-api-openapi.yml
- filename: aza-finance-payout-methods-api-openapi.yml
  format: yaml
  label: AZA Finance Payout Methods API
  slug: aza-finance-payout-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-payout-methods-api-openapi.yml
- filename: aza-finance-recipients-api-openapi.yml
  format: yaml
  label: AZA Finance Recipients API
  slug: aza-finance-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-recipients-api-openapi.yml
- filename: aza-finance-senders-api-openapi.yml
  format: yaml
  label: AZA Finance Senders API
  slug: aza-finance-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-senders-api-openapi.yml
- filename: aza-finance-transactions-api-openapi.yml
  format: yaml
  label: AZA Finance Transactions API
  slug: aza-finance-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-transactions-api-openapi.yml
- filename: aza-finance-webhooks-api-openapi.yml
  format: yaml
  label: AZA Finance Webhooks API
  slug: aza-finance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/openapi/aza-finance-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azafinance.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: transferzero.com
  spf: true
hosts:
- cert_expires: Oct  9 03:37:43 2026 GMT
  host: www.azafinance.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:46:24 2026 GMT
  host: api-sandbox.transferzero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 04:46:24 2026 GMT
  host: api.transferzero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aza Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AZA Finance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AZA Finance
provider_slug: aza-finance
slug: aza-finance-domain-security
source_filename: aza-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.azafinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 03:37:43 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api-sandbox.transferzero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:46:24 2026 GMT\n  hsts: null\n- host: api.transferzero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 04:46:24 2026 GMT\n  hsts: null\ndomains:\n- domain: azafinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: transferzero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aza-finance/refs/heads/main/security/aza-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Payments
- Foreign Exchange
- Cross-Border Payments
- Africa
- Fintech
- API
---
