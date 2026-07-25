---
api_specs:
- filename: lead-bank-account-number-api-openapi.yml
  format: yaml
  label: Lead Bank Account Number API
  slug: lead-bank-account-number-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-account-number-api-openapi.yml
- filename: lead-bank-ach-api-openapi.yml
  format: yaml
  label: Lead Bank ACH API
  slug: lead-bank-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-ach-api-openapi.yml
- filename: lead-bank-blockchain-payment-api-openapi.yml
  format: yaml
  label: Lead Bank Blockchain Payment API
  slug: lead-bank-blockchain-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-blockchain-payment-api-openapi.yml
- filename: lead-bank-compliance-api-openapi.yml
  format: yaml
  label: Lead Bank Compliance API
  slug: lead-bank-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-compliance-api-openapi.yml
- filename: lead-bank-entity-api-openapi.yml
  format: yaml
  label: Lead Bank Entity API
  slug: lead-bank-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-entity-api-openapi.yml
- filename: lead-bank-events-api-openapi.yml
  format: yaml
  label: Lead Bank Events API
  slug: lead-bank-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-events-api-openapi.yml
- filename: lead-bank-funding-api-openapi.yml
  format: yaml
  label: Lead Bank Funding API
  slug: lead-bank-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-funding-api-openapi.yml
- filename: lead-bank-instant-payments-api-openapi.yml
  format: yaml
  label: Lead Bank Instant Payments API
  slug: lead-bank-instant-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-instant-payments-api-openapi.yml
- filename: lead-bank-internal-transfer-api-openapi.yml
  format: yaml
  label: Lead Bank Internal Transfer API
  slug: lead-bank-internal-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-internal-transfer-api-openapi.yml
- filename: lead-bank-lending-api-openapi.yml
  format: yaml
  label: Lead Bank Lending API
  slug: lead-bank-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-lending-api-openapi.yml
- filename: lead-bank-lending-simulation-api-openapi.yml
  format: yaml
  label: Lead Bank Lending Simulation API
  slug: lead-bank-lending-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-lending-simulation-api-openapi.yml
- filename: lead-bank-oauth-api-openapi.yml
  format: yaml
  label: Lead Bank OAuth API
  slug: lead-bank-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-oauth-api-openapi.yml
- filename: lead-bank-originator-api-openapi.yml
  format: yaml
  label: Lead Bank Originator API
  slug: lead-bank-originator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-originator-api-openapi.yml
- filename: lead-bank-simulation-api-openapi.yml
  format: yaml
  label: Lead Bank Simulation API
  slug: lead-bank-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-simulation-api-openapi.yml
- filename: lead-bank-subledger-balances-api-openapi.yml
  format: yaml
  label: Lead Bank Subledger Balances API
  slug: lead-bank-subledger-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-subledger-balances-api-openapi.yml
- filename: lead-bank-wire-api-openapi.yml
  format: yaml
  label: Lead Bank Wire API
  slug: lead-bank-wire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/openapi/lead-bank-wire-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lead.bank
  spf: true
hosts:
- cert_expires: Sep 23 00:58:37 2026 GMT
  host: lead.bank
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 12:24:08 2026 GMT
  host: docs.lead.bank
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.sandbox.lead.bank
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lead Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lead Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lead Bank
provider_slug: lead-bank
slug: lead-bank-domain-security
source_filename: lead-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lead.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 00:58:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lead.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 12:24:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sandbox.lead.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lead.bank\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/security/lead-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Sponsor Bank
- Embedded Finance
- Banking as a Service
- Payments
- Lending
- Cards
- Deposits
---
