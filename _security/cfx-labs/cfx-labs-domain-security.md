---
api_specs:
- filename: cfx-labs-cash-api-openapi.yml
  format: yaml
  label: CFX Labs Cash API
  slug: cfx-labs-cash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-cash-api-openapi.yml
- filename: cfx-labs-deposit-api-openapi.yml
  format: yaml
  label: CFX Labs Deposit API
  slug: cfx-labs-deposit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-deposit-api-openapi.yml
- filename: cfx-labs-deposit-memos-api-openapi.yml
  format: yaml
  label: CFX Labs Deposit Memos API
  slug: cfx-labs-deposit-memos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-deposit-memos-api-openapi.yml
- filename: cfx-labs-escrow-transfers-api-openapi.yml
  format: yaml
  label: CFX Labs Escrow Transfers API
  slug: cfx-labs-escrow-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-escrow-transfers-api-openapi.yml
- filename: cfx-labs-identity-api-openapi.yml
  format: yaml
  label: CFX Labs Identity API
  slug: cfx-labs-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-identity-api-openapi.yml
- filename: cfx-labs-identity-documents-api-openapi.yml
  format: yaml
  label: CFX Labs Identity Documents API
  slug: cfx-labs-identity-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-identity-documents-api-openapi.yml
- filename: cfx-labs-ledger-accounts-api-openapi.yml
  format: yaml
  label: CFX Labs Ledger Accounts API
  slug: cfx-labs-ledger-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-ledger-accounts-api-openapi.yml
- filename: cfx-labs-payment-instruments-api-openapi.yml
  format: yaml
  label: CFX Labs Payment Instruments API
  slug: cfx-labs-payment-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-payment-instruments-api-openapi.yml
- filename: cfx-labs-products-api-openapi.yml
  format: yaml
  label: CFX Labs Products API
  slug: cfx-labs-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-products-api-openapi.yml
- filename: cfx-labs-transfer-requests-api-openapi.yml
  format: yaml
  label: CFX Labs Transfer Requests API
  slug: cfx-labs-transfer-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-transfer-requests-api-openapi.yml
- filename: cfx-labs-us-bank-ach-api-openapi.yml
  format: yaml
  label: CFX Labs US Bank ACH API
  slug: cfx-labs-us-bank-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/openapi/cfx-labs-us-bank-ach-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cfx.to
  spf: true
hosts:
- cert_expires: Apr 13 23:59:59 2027 GMT
  host: cfx.to
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cfx Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CFX Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CFX Labs
provider_slug: cfx-labs
slug: cfx-labs-domain-security
source_filename: cfx-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cfx.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cfx.to\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cfx-labs/refs/heads/main/security/cfx-labs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- fintech
- banking
- payments
- API
- programmable
- company
---
