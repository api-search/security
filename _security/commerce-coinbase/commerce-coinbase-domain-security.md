---
api_specs:
- filename: openapi-charges.yml
  format: yaml
  label: Coinbase Commerce Charges API
  slug: coinbase-commerce-charges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commerce-coinbase/refs/heads/main/openapi/openapi-charges.yml
- filename: openapi-checkouts.yml
  format: yaml
  label: Coinbase Business Checkouts API
  slug: coinbase-business-checkouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commerce-coinbase/refs/heads/main/openapi/openapi-checkouts.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@coinbase.com"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coinbase.com
  spf: true
hosts:
- cert_expires: Sep  8 09:01:10 2026 GMT
  host: commerce.coinbase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 09:01:10 2026 GMT
  host: api.commerce.coinbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: docs.cdp.coinbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commerce Coinbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinbase Commerce, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coinbase Commerce
provider_slug: commerce-coinbase
slug: commerce-coinbase-domain-security
source_filename: commerce-coinbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commerce.coinbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:01:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.commerce.coinbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:01:10 2026 GMT\n  hsts: null\n- host: docs.cdp.coinbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coinbase.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@coinbase.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commerce-coinbase/refs/heads/main/security/commerce-coinbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crypto Payments
- Cryptocurrency
- Payment Gateway
- Commerce
- Bitcoin
- Ethereum
- USDC
- Webhooks
- Charges
- Checkouts
---
