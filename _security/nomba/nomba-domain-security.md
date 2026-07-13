---
api_specs:
- filename: nomba-authentication-openapi.yml
  format: yaml
  label: Nomba Authentication API
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-authentication-openapi.yml
- filename: nomba-accounts-openapi.yml
  format: yaml
  label: Nomba Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-accounts-openapi.yml
- filename: nomba-virtual-accounts-openapi.yml
  format: yaml
  label: Nomba Virtual Accounts API
  slug: virtual-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-virtual-accounts-openapi.yml
- filename: nomba-transfers-openapi.yml
  format: yaml
  label: Nomba Transfers API
  slug: transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-transfers-openapi.yml
- filename: nomba-online-checkout-openapi.yml
  format: yaml
  label: Nomba Online Checkout API
  slug: online-checkout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-online-checkout-openapi.yml
- filename: nomba-charge-openapi.yml
  format: yaml
  label: Nomba Charge API
  slug: charge
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-charge-openapi.yml
- filename: nomba-transactions-openapi.yml
  format: yaml
  label: Nomba Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-transactions-openapi.yml
- filename: nomba-global-payout-openapi.yml
  format: yaml
  label: Nomba Global Payout API
  slug: global-payout
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/openapi/nomba-global-payout-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nomba.com
  spf: true
hosts:
- cert_expires: Aug 18 18:47:32 2026 GMT
  host: nomba.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 10:39:02 2026 GMT
  host: developer.nomba.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 10:39:02 2026 GMT
  host: api.nomba.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nomba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomba, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nomba
provider_slug: nomba
slug: nomba-domain-security
source_filename: nomba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nomba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 18:47:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: developer.nomba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:39:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nomba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:39:02 2026 GMT\n  hsts: null\ndomains:\n- domain: nomba.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomba/refs/heads/main/security/nomba-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fintech
- Banking
- Transfers
- Virtual Accounts
- Checkout
- Cross-Border Payments
- Cards
---
