---
api_specs:
- filename: fdx-account-information-api-openapi.yml
  format: yaml
  label: Financial Data Exchange (FDX) Account Information API
  slug: fdx-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fdx/refs/heads/main/openapi/fdx-account-information-api-openapi.yml
- filename: fdx-account-statements-api-openapi.yml
  format: yaml
  label: Financial Data Exchange (FDX) Account Statements API
  slug: fdx-account-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fdx/refs/heads/main/openapi/fdx-account-statements-api-openapi.yml
- filename: fdx-account-transactions-api-openapi.yml
  format: yaml
  label: Financial Data Exchange (FDX) Account Transactions API
  slug: fdx-account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fdx/refs/heads/main/openapi/fdx-account-transactions-api-openapi.yml
- filename: fdx-asset-transfer-networks-information-api-openapi.yml
  format: yaml
  label: Financial Data Exchange (FDX) Asset Transfer Networks Information API
  slug: fdx-asset-transfer-networks-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fdx/refs/heads/main/openapi/fdx-asset-transfer-networks-information-api-openapi.yml
- filename: fdx-payment-networks-information-api-openapi.yml
  format: yaml
  label: Financial Data Exchange (FDX) Payment Networks Information API
  slug: fdx-payment-networks-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fdx/refs/heads/main/openapi/fdx-payment-networks-information-api-openapi.yml
- filename: fdx-personal-information-api-openapi.yml
  format: yaml
  label: Financial Data Exchange (FDX) Personal Information API
  slug: fdx-personal-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fdx/refs/heads/main/openapi/fdx-personal-information-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: financialdataexchange.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-organization.com
  spf: false
hosts:
- cert_expires: Sep 18 08:08:34 2026 GMT
  host: financialdataexchange.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.financialdataexchange.org
  https: false
- host: api.your-organization.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fdx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Financial Data Exchange (FDX), probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Financial Data Exchange (FDX)
provider_slug: fdx
slug: fdx-domain-security
source_filename: fdx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: financialdataexchange.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:08:34 2026 GMT\n  hsts: false\n- host: api.financialdataexchange.org\n  https: false\n- host: api.your-organization.com\n  https: false\ndomains:\n- domain: financialdataexchange.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: your-organization.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fdx/refs/heads/main/security/fdx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Data
- Open Banking
- Open Finance
- Financial Data Exchange
- Consumer Permissioned
- Account Data
- Transaction
- Investments
- Insurance
- Tax Data
- Payroll
- REST
- Authentication
- FAPI
- CFPB 1033
---
