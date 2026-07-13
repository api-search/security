---
api_specs:
- filename: coinbase-advanced-trade-openapi.yml
  format: yaml
  label: Coinbase Advanced Trade API
  slug: advanced-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/openapi/coinbase-advanced-trade-openapi.yml
- filename: coinbase-exchange-openapi.yml
  format: yaml
  label: Coinbase Exchange API
  slug: exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/openapi/coinbase-exchange-openapi.yml
- filename: coinbase-prime-openapi.yml
  format: yaml
  label: Coinbase Prime API
  slug: prime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/openapi/coinbase-prime-openapi.yml
- filename: coinbase-onramp-openapi.yml
  format: yaml
  label: Coinbase Onramp API
  slug: onramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/openapi/coinbase-onramp-openapi.yml
- filename: coinbase-commerce-openapi.yml
  format: yaml
  label: Coinbase Commerce API
  slug: commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/openapi/coinbase-commerce-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@coinbase.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coinbase.com
  spf: true
hosts:
- cert_expires: Oct  4 03:37:00 2026 GMT
  host: www.coinbase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: docs.cdp.coinbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 03:37:00 2026 GMT
  host: api.coinbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinbase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coinbase
provider_slug: coinbase
slug: coinbase-domain-security
source_filename: coinbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coinbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 03:37:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cdp.coinbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.coinbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 03:37:00 2026 GMT\n  hsts: null\ndomains:\n- domain: coinbase.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@coinbase.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinbase/refs/heads/main/security/coinbase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Cryptocurrency
- Custody
- Exchange
- Onramp
- Payments
- Trading
- Wallet
- Web3
---
