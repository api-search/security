---
api_specs:
- filename: zenledger-authentication-api-openapi.yml
  format: yaml
  label: ZenLedger Authentication API
  slug: zenledger-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-authentication-api-openapi.yml
- filename: zenledger-companies-api-openapi.yml
  format: yaml
  label: ZenLedger Companies API
  slug: zenledger-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-companies-api-openapi.yml
- filename: zenledger-holdings-api-openapi.yml
  format: yaml
  label: ZenLedger Holdings API
  slug: zenledger-holdings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-holdings-api-openapi.yml
- filename: zenledger-imports-api-openapi.yml
  format: yaml
  label: ZenLedger Imports API
  slug: zenledger-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-imports-api-openapi.yml
- filename: zenledger-polymarkets-api-openapi.yml
  format: yaml
  label: ZenLedger Polymarkets API
  slug: zenledger-polymarkets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-polymarkets-api-openapi.yml
- filename: zenledger-portfolios-api-openapi.yml
  format: yaml
  label: ZenLedger Portfolios API
  slug: zenledger-portfolios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-portfolios-api-openapi.yml
- filename: zenledger-supported-chains-api-openapi.yml
  format: yaml
  label: ZenLedger Supported Chains API
  slug: zenledger-supported-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-supported-chains-api-openapi.yml
- filename: zenledger-supported-currencies-api-openapi.yml
  format: yaml
  label: ZenLedger Supported Currencies API
  slug: zenledger-supported-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-supported-currencies-api-openapi.yml
- filename: zenledger-supported-exchanges-and-wallets-api-openapi.yml
  format: yaml
  label: ZenLedger Supported Exchanges and Wallets API
  slug: zenledger-supported-exchanges-and-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-supported-exchanges-and-wallets-api-openapi.yml
- filename: zenledger-taxes-api-openapi.yml
  format: yaml
  label: ZenLedger Taxes API
  slug: zenledger-taxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-taxes-api-openapi.yml
- filename: zenledger-transactions-api-openapi.yml
  format: yaml
  label: ZenLedger Transactions API
  slug: zenledger-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-transactions-api-openapi.yml
- filename: zenledger-users-api-openapi.yml
  format: yaml
  label: ZenLedger Users API
  slug: zenledger-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-users-api-openapi.yml
- filename: zenledger-wallet-screening-api-openapi.yml
  format: yaml
  label: ZenLedger Wallet Screening API
  slug: zenledger-wallet-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/openapi/zenledger-wallet-screening-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zenledger.io
  spf: true
hosts:
- cert_expires: Nov 24 20:16:20 2026 GMT
  host: zenledger.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:25:31 2026 GMT
  host: docs.zenledger.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 06:11:07 2026 GMT
  host: api.zenledger.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Zenledger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZenLedger, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ZenLedger
provider_slug: zenledger
slug: zenledger-domain-security
source_filename: zenledger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenledger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 20:16:20 2026 GMT\n  hsts: null\n- host: docs.zenledger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:25:31 2026 GMT\n  hsts: false\n- host: api.zenledger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 06:11:07 2026 GMT\n  hsts: null\ndomains:\n- domain: zenledger.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenledger/refs/heads/main/security/zenledger-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Crypto Tax
- Digital Assets
- Tax Compliance
- Blockchain Analytics
- RegTech
- Accounting
- Sanctions Screening
- Financial Services
- Portfolio Aggregation
- Cryptocurrency
---
