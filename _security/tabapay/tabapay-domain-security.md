---
api_specs:
- filename: tabapay-3d-secure-api-openapi.yml
  format: yaml
  label: TabaPay 3D Secure API
  slug: tabapay-3d-secure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-3d-secure-api-openapi.yml
- filename: tabapay-account-api-openapi.yml
  format: yaml
  label: TabaPay Account API
  slug: tabapay-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-account-api-openapi.yml
- filename: tabapay-bank-api-openapi.yml
  format: yaml
  label: TabaPay Bank API
  slug: tabapay-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-bank-api-openapi.yml
- filename: tabapay-card-api-openapi.yml
  format: yaml
  label: TabaPay Card API
  slug: tabapay-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-card-api-openapi.yml
- filename: tabapay-client-api-openapi.yml
  format: yaml
  label: TabaPay Client API
  slug: tabapay-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-client-api-openapi.yml
- filename: tabapay-fxrate-api-openapi.yml
  format: yaml
  label: TabaPay FXRate API
  slug: tabapay-fxrate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-fxrate-api-openapi.yml
- filename: tabapay-health-api-openapi.yml
  format: yaml
  label: TabaPay Health API
  slug: tabapay-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-health-api-openapi.yml
- filename: tabapay-key-api-openapi.yml
  format: yaml
  label: TabaPay Key API
  slug: tabapay-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-key-api-openapi.yml
- filename: tabapay-ledger-api-openapi.yml
  format: yaml
  label: TabaPay Ledger API
  slug: tabapay-ledger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-ledger-api-openapi.yml
- filename: tabapay-ofac-api-openapi.yml
  format: yaml
  label: TabaPay OFAC API
  slug: tabapay-ofac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-ofac-api-openapi.yml
- filename: tabapay-subclient-api-openapi.yml
  format: yaml
  label: TabaPay SubClient API
  slug: tabapay-subclient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-subclient-api-openapi.yml
- filename: tabapay-tag-api-openapi.yml
  format: yaml
  label: TabaPay Tag API
  slug: tabapay-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-tag-api-openapi.yml
- filename: tabapay-transaction-api-openapi.yml
  format: yaml
  label: TabaPay Transaction API
  slug: tabapay-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-transaction-api-openapi.yml
- filename: tabapay-transactionrequest-api-openapi.yml
  format: yaml
  label: TabaPay TransactionRequest API
  slug: tabapay-transactionrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-transactionrequest-api-openapi.yml
- filename: tabapay-user-api-openapi.yml
  format: yaml
  label: TabaPay User API
  slug: tabapay-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-user-api-openapi.yml
- filename: tabapay-verification-api-openapi.yml
  format: yaml
  label: TabaPay Verification API
  slug: tabapay-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/openapi/tabapay-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tabapay.com
  spf: true
hosts:
- cert_expires: Sep 26 22:43:30 2026 GMT
  host: tabapay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 08:46:22 2026 GMT
  host: developers.tabapay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.tabapay.com
  https: false
kind: domain-security
layout: security
method: probed
name: Tabapay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TabaPay, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TabaPay
provider_slug: tabapay
slug: tabapay-domain-security
source_filename: tabapay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tabapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:43:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.tabapay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:46:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tabapay.com\n  https: false\ndomains:\n- domain: tabapay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabapay/refs/heads/main/security/tabapay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Instant Payments
- Money Movement
- Payouts
- Cards
- Real-Time Payments
- ACH
---
