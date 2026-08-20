---
api_specs:
- filename: opennode-charges-api-openapi.yml
  format: yaml
  label: OpenNode Charges API
  slug: opennode-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-charges-api-openapi.yml
- filename: opennode-withdrawals-api-openapi.yml
  format: yaml
  label: OpenNode Withdrawals API
  slug: opennode-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-withdrawals-api-openapi.yml
- filename: opennode-refunds-api-openapi.yml
  format: yaml
  label: OpenNode Refunds API
  slug: opennode-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-refunds-api-openapi.yml
- filename: opennode-account-api-openapi.yml
  format: yaml
  label: OpenNode Account API
  slug: opennode-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-account-api-openapi.yml
- filename: opennode-static-addresses-api-openapi.yml
  format: yaml
  label: OpenNode Static Addresses API
  slug: opennode-static-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-static-addresses-api-openapi.yml
- filename: opennode-account-api-openapi.yml
  format: yaml
  label: OpenNode Account API
  slug: opennode-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-account-api-openapi.yml
- filename: opennode-charges-api-openapi.yml
  format: yaml
  label: OpenNode Charges API
  slug: opennode-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-charges-api-openapi.yml
- filename: opennode-rates-api-openapi.yml
  format: yaml
  label: OpenNode Rates API
  slug: opennode-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-rates-api-openapi.yml
- filename: opennode-refunds-api-openapi.yml
  format: yaml
  label: OpenNode Refunds API
  slug: opennode-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-refunds-api-openapi.yml
- filename: opennode-static-addresses-api-openapi.yml
  format: yaml
  label: OpenNode Static Addresses API
  slug: opennode-static-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-static-addresses-api-openapi.yml
- filename: opennode-withdrawals-api-openapi.yml
  format: yaml
  label: OpenNode Withdrawals API
  slug: opennode-withdrawals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/openapi/opennode-withdrawals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opennode.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: opennode.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 10:57:47 2026 GMT
  host: developers.opennode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.opennode.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opennode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenNode, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenNode
provider_slug: opennode
slug: opennode-domain-security
source_filename: opennode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opennode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: false\n- host: developers.opennode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:57:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.opennode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: opennode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opennode/refs/heads/main/security/opennode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bitcoin
- Lightning Network
- Payments
- Payment Processing
- Cryptocurrency
- Fintech
- Webhook
- Invoicing
- Payouts
- LNURL
---
