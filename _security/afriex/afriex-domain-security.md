---
api_specs:
- filename: afriex-balance-api-openapi.yml
  format: yaml
  label: Afriex Balance API
  slug: afriex-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-balance-api-openapi.yml
- filename: afriex-checkout-sessions-api-openapi.yml
  format: yaml
  label: Afriex Checkout Sessions API
  slug: afriex-checkout-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-checkout-sessions-api-openapi.yml
- filename: afriex-customers-api-openapi.yml
  format: yaml
  label: Afriex Customers API
  slug: afriex-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-customers-api-openapi.yml
- filename: afriex-media-api-openapi.yml
  format: yaml
  label: Afriex Media API
  slug: afriex-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-media-api-openapi.yml
- filename: afriex-payment-methods-api-openapi.yml
  format: yaml
  label: Afriex Payment Methods API
  slug: afriex-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-payment-methods-api-openapi.yml
- filename: afriex-rates-api-openapi.yml
  format: yaml
  label: Afriex Rates API
  slug: afriex-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-rates-api-openapi.yml
- filename: afriex-sme-registration-api-openapi.yml
  format: yaml
  label: Afriex SME Registration API
  slug: afriex-sme-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-sme-registration-api-openapi.yml
- filename: afriex-transactions-api-openapi.yml
  format: yaml
  label: Afriex Transactions API
  slug: afriex-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-transactions-api-openapi.yml
- filename: afriex-webhooks-api-openapi.yml
  format: yaml
  label: Afriex Webhooks API
  slug: afriex-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/openapi/afriex-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  caa_note: No CAA records published; re-queried against 1.1.1.1 and 8.8.8.8 on 2026-09-12, both returned an empty answer (the initial probe recorded a resolver timeout string, corrected here to the measured empty result).
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: afriex.com
  spf: true
hosts:
- cert_expires: Dec 10 06:14:06 2026 GMT
  host: www.afriex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 18:44:11 2026 GMT
  host: docs.afriex.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 01:01:14 2026 GMT
  host: api.afriex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Afriex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Afriex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Afriex
provider_slug: afriex
slug: afriex-domain-security
source_filename: afriex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.afriex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:14:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.afriex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:44:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.afriex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 01:01:14 2026 GMT\n  hsts: null\ndomains:\n- domain: afriex.com\n  dnssec: false\n  caa: []\n  caa_note: 'No CAA records published; re-queried against 1.1.1.1 and 8.8.8.8 on 2026-09-12,\n    both returned an empty answer (the initial probe recorded a resolver timeout string,\n    corrected here to the measured empty result).'\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afriex/refs/heads/main/security/afriex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Remittances
- Cross-Border Payments
- Fintech
- Financial Services
- Foreign Exchange
- Mobile Money
- Money Transfer
- Africa
- Stablecoins
- Virtual Accounts
- Webhook
- A2A
---
