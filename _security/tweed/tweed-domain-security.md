---
api_specs:
- filename: tweed-assets-api-openapi.yml
  format: yaml
  label: Tweed assets API
  slug: tweed-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-assets-api-openapi.yml
- filename: tweed-audit-event-mappings-api-openapi.yml
  format: yaml
  label: Tweed audit-event-mappings API
  slug: tweed-audit-event-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-audit-event-mappings-api-openapi.yml
- filename: tweed-auth-api-openapi.yml
  format: yaml
  label: Tweed auth API
  slug: tweed-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-auth-api-openapi.yml
- filename: tweed-blockchains-api-openapi.yml
  format: yaml
  label: Tweed blockchains API
  slug: tweed-blockchains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-blockchains-api-openapi.yml
- filename: tweed-checkout-api-openapi.yml
  format: yaml
  label: Tweed checkout API
  slug: tweed-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-checkout-api-openapi.yml
- filename: tweed-contracts-api-openapi.yml
  format: yaml
  label: Tweed contracts API
  slug: tweed-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-contracts-api-openapi.yml
- filename: tweed-items-api-openapi.yml
  format: yaml
  label: Tweed items API
  slug: tweed-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-items-api-openapi.yml
- filename: tweed-payouts-api-openapi.yml
  format: yaml
  label: Tweed payouts API
  slug: tweed-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-payouts-api-openapi.yml
- filename: tweed-platform-webhooks-api-openapi.yml
  format: yaml
  label: Tweed platform-webhooks API
  slug: tweed-platform-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-platform-webhooks-api-openapi.yml
- filename: tweed-rate-api-openapi.yml
  format: yaml
  label: Tweed Rate API
  slug: tweed-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-rate-api-openapi.yml
- filename: tweed-tickets-api-openapi.yml
  format: yaml
  label: Tweed tickets API
  slug: tweed-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/openapi/tweed-tickets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: paytweed.com
  spf: true
hosts:
- cert_expires: Sep 27 06:12:00 2026 GMT
  host: www.paytweed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 20:17:40 2026 GMT
  host: docs.paytweed.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: api-v2.prod.paytweed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tweed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tweed, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Tweed
provider_slug: tweed
slug: tweed-domain-security
source_filename: tweed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paytweed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:12:00 2026 GMT\n  hsts: null\n- host: docs.paytweed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:17:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-v2.prod.paytweed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: paytweed.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tweed/refs/heads/main/security/tweed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Crypto
- Wallets
- NFT
- Blockchain
- Web3
- Checkout
---
