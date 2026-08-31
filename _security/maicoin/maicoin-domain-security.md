---
api_specs:
- filename: maicoin-convert-api-openapi.yml
  format: yaml
  label: MaiCoin Convert API
  slug: maicoin-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maicoin/refs/heads/main/openapi/maicoin-convert-api-openapi.yml
- filename: maicoin-order-api-openapi.yml
  format: yaml
  label: MaiCoin Order API
  slug: maicoin-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maicoin/refs/heads/main/openapi/maicoin-order-api-openapi.yml
- filename: maicoin-public-api-openapi.yml
  format: yaml
  label: MaiCoin Public API
  slug: maicoin-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maicoin/refs/heads/main/openapi/maicoin-public-api-openapi.yml
- filename: maicoin-trade-api-openapi.yml
  format: yaml
  label: MaiCoin Trade API
  slug: maicoin-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maicoin/refs/heads/main/openapi/maicoin-trade-api-openapi.yml
- filename: maicoin-transaction-api-openapi.yml
  format: yaml
  label: MaiCoin Transaction API
  slug: maicoin-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maicoin/refs/heads/main/openapi/maicoin-transaction-api-openapi.yml
- filename: maicoin-user-api-openapi.yml
  format: yaml
  label: MaiCoin User API
  slug: maicoin-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maicoin/refs/heads/main/openapi/maicoin-user-api-openapi.yml
- filename: maicoin-wallet-api-openapi.yml
  format: yaml
  label: MaiCoin Wallet API
  slug: maicoin-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maicoin/refs/heads/main/openapi/maicoin-wallet-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@maicoin.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: maicoin.com
  spf: true
hosts:
- cert_expires: Sep  7 23:59:59 2026 GMT
  host: max.maicoin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 04:04:28 2026 GMT
  host: campaign.maicoin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 23:59:59 2026 GMT
  host: max-api.maicoin.com
  hsts: partial
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_note: 'PATH-DEPENDENT, corrected after the automated probe. The probe reads the host ROOT, which returns 200 with NO strict-transport-security header, so it recorded hsts:false. A follow-up probe on 2026-08-25 of the actual API paths (GET /api/v3/timestamp and /api/v3/markets) DID return `strict-transport-security: max-age=63072000; includeSubDomains`. HSTS is therefore enforced on the API surface but absent on the bare host, which is a real (minor) gap: a first contact with https://max-api.maicoin.com/ is not pinned.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maicoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MaiCoin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MaiCoin
provider_slug: maicoin
slug: maicoin-domain-security
source_filename: maicoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: max.maicoin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 23:59:59 2026 GMT\n  hsts: null\n- host: campaign.maicoin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 04:04:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: max-api.maicoin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 23:59:59 2026 GMT\n  hsts: partial\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    PATH-DEPENDENT, corrected after the automated probe. The probe reads the host ROOT, which\n    returns 200 with NO strict-transport-security header, so it recorded hsts:false. A follow-up\n    probe on 2026-08-25 of the actual API paths (GET /api/v3/timestamp and /api/v3/markets) DID\n    return `strict-transport-security: max-age=63072000; includeSubDomains`. HSTS is therefore\n    enforced on the\
  \ API surface but absent on the bare host, which is a real (minor) gap: a first\n    contact with https://max-api.maicoin.com/ is not pinned.\ndomains:\n- domain: maicoin.com\n  dnssec: true\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@maicoin.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maicoin/refs/heads/main/security/maicoin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Digital Assets
- Exchange
- Trading
- Financial Services
- Market Data
- Blockchain
- Taiwan
- WebSocket
---
