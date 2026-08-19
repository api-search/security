---
api_specs:
- filename: memo-bank-premium-bank-api-openapi.yml
  format: yaml
  label: Memo Bank Premium Bank API
  slug: memo-bank-premium-bank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-premium-bank-api-openapi.yml
- filename: memo-bank-marketplace-api-openapi.yml
  format: yaml
  label: Memo Bank Marketplace API
  slug: memo-bank-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-marketplace-api-openapi.yml
- filename: memo-bank-nextgenpsd2-api-openapi.yml
  format: yaml
  label: Memo Bank NextGenPSD2 API
  slug: memo-bank-nextgenpsd2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-nextgenpsd2-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@memo.bank"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: memo.bank
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: memo.bank
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 21:41:19 2026 GMT
  host: docs.api.memo.bank
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 15:23:01 2026 GMT
  host: api.memo.bank
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memo Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memo Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Memo Bank
provider_slug: memo-bank
slug: memo-bank-domain-security
source_filename: memo-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memo.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\n- host: docs.api.memo.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:41:19 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.memo.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 15:23:01 2026 GMT\n  hsts: null\ndomains:\n- domain: memo.bank\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@memo.bank\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/security/memo-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech Insurtech
- banking
- business-banking
- payments
- sepa
- sepa-direct-debit
- virtual-iban
- wire-transfers
- open-banking
- psd2
- berlin-group
- webhooks
- mcp
- france
---
