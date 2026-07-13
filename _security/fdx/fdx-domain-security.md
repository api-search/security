---
api_specs:
- filename: core-exchange
  format: yaml
  label: FDX Accounts API
  slug: fdx-accounts-api
  spec_type: OpenAPI
  url: https://github.com/plaid/core-exchange
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
- Transactions
- Investments
- Insurance
- Tax Data
- Payroll
- REST
- OAuth2
- FAPI
- CFPB 1033
---
