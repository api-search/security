---
api_specs:
- filename: paywithmybank-accountdata-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) accountData API
  slug: paywithmybank-accountdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-accountdata-api-openapi.yml
- filename: paywithmybank-accounts-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) accounts API
  slug: paywithmybank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-accounts-api-openapi.yml
- filename: paywithmybank-countries-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) countries API
  slug: paywithmybank-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-countries-api-openapi.yml
- filename: paywithmybank-customers-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) customers API
  slug: paywithmybank-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-customers-api-openapi.yml
- filename: paywithmybank-disputemanagement-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) disputeManagement API
  slug: paywithmybank-disputemanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-disputemanagement-api-openapi.yml
- filename: paywithmybank-identity-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) identity API
  slug: paywithmybank-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-identity-api-openapi.yml
- filename: paywithmybank-networkcheckapi-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) networkCheckApi API
  slug: paywithmybank-networkcheckapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-networkcheckapi-api-openapi.yml
- filename: paywithmybank-paymentproviders-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) paymentProviders API
  slug: paywithmybank-paymentproviders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-paymentproviders-api-openapi.yml
- filename: paywithmybank-payments-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) payments API
  slug: paywithmybank-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-payments-api-openapi.yml
- filename: paywithmybank-transactions-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) transactions API
  slug: paywithmybank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-transactions-api-openapi.yml
- filename: paywithmybank-verifycustomer-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) verifyCustomer API
  slug: paywithmybank-verifycustomer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-verifycustomer-api-openapi.yml
- filename: paywithmybank-api-api-openapi.yml
  format: yaml
  label: PayWithMyBank (Trustly) API
  slug: paywithmybank-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/openapi/paywithmybank-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paywithmybank.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.paywithmybank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paywithmybank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayWithMyBank (Trustly), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PayWithMyBank (Trustly)
provider_slug: paywithmybank
slug: paywithmybank-domain-security
source_filename: paywithmybank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paywithmybank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paywithmybank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paywithmybank/refs/heads/main/security/paywithmybank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Pay by Bank
- Open Banking
- ACH
- Bank Transfers
- Fintech
- Identity Verification
- Webhook
---
