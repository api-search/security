---
api_specs:
- filename: ripple-labs-rlusd-openapi-original.yml
  format: yaml
  label: Ripple Mint API (RLUSD Stablecoin)
  slug: ripple-mint-api-rlusd-stablecoin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-rlusd-openapi-original.yml
- filename: ripple-labs-ripplenet-openapi-original.yml
  format: yaml
  label: RippleNet Server API
  slug: ripplenet-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-ripplenet-openapi-original.yml
- filename: ripple-labs-report-service-openapi-original.yml
  format: yaml
  label: Report Service API
  slug: report-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-report-service-openapi-original.yml
- filename: ripple-labs-smart-liquidation-openapi-original.yml
  format: yaml
  label: Smart Liquidation API
  slug: smart-liquidation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-smart-liquidation-openapi-original.yml
- filename: ripple-labs-palisade-wallet-openapi-original.yml
  format: yaml
  label: Palisade Wallet-as-a-Service API
  slug: palisade-wallet-as-a-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/openapi/ripple-labs-palisade-wallet-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ripple.com
  spf: true
hosts:
- cert_expires: Sep  3 09:23:46 2026 GMT
  host: ripple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 15:13:10 2026 GMT
  host: docs.ripple.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 15:06:54 2026 GMT
  host: api.ripple.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ripple Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ripple Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ripple Labs
provider_slug: ripple-labs
slug: ripple-labs-domain-security
source_filename: ripple-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ripple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:23:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ripple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:13:10 2026 GMT\n  hsts: false\n- host: api.ripple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:06:54 2026 GMT\n  hsts: null\ndomains:\n- domain: ripple.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripple-labs/refs/heads/main/security/ripple-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Payments
- Cross-Border Payments
- Blockchain
- Cryptocurrency
- Stablecoin
- Digital Assets
- Custody
- Wallet
- Fintech
---
