---
api_specs:
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Accounts API
  slug: increase-com-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Account Numbers API
  slug: increase-com-account-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Cards API
  slug: increase-com-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Card Payments API
  slug: increase-com-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase ACH Transfers API
  slug: increase-com-ach-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Wire Transfers API
  slug: increase-com-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Real-Time Payments API
  slug: increase-com-real-time-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Checks API
  slug: increase-com-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Transactions API
  slug: increase-com-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Entities API
  slug: increase-com-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Events and Webhooks API
  slug: increase-com-events-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Bookkeeping API
  slug: increase-com-bookkeeping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Card Profiles and Digital Wallets API
  slug: increase-com-card-profiles-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Lockboxes API
  slug: increase-com-lockboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
- filename: increase-com-openapi.yml
  format: yaml
  label: Increase Simulations API
  slug: increase-com-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/openapi/increase-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: increase.com
  spf: true
hosts:
- cert_expires: Sep 17 00:37:53 2026 GMT
  host: increase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 03:41:37 2026 GMT
  host: api.increase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 12:59:59 2026 GMT
  host: sandbox.increase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Increase Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Increase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Increase
provider_slug: increase-com
slug: increase-com-domain-security
source_filename: increase-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: increase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 00:37:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.increase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:41:37 2026 GMT\n  hsts: null\n- host: sandbox.increase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 12:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: increase.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/increase-com/refs/heads/main/security/increase-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Banking
- Financial Infrastructure
- ACH
- Wire Transfers
- Real-Time Payments
- Cards
- Fintech
---
