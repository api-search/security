---
api_specs:
- filename: tvarka-atk-api-auth-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Auth API
  slug: tvarka-atk-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-auth-api-openapi.yml
- filename: tvarka-atk-api-erasure-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Erasure API
  slug: tvarka-atk-api-erasure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-erasure-api-openapi.yml
- filename: tvarka-atk-api-ltv-api-openapi.yml
  format: yaml
  label: Tvarka ATK API LTV API
  slug: tvarka-atk-api-ltv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-ltv-api-openapi.yml
- filename: tvarka-atk-api-pairing-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Pairing API
  slug: tvarka-atk-api-pairing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-pairing-api-openapi.yml
- filename: tvarka-atk-api-sign-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Sign API
  slug: tvarka-atk-api-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-sign-api-openapi.yml
- filename: tvarka-atk-api-tvarka-atk-api-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Tvarka ATK API API
  slug: tvarka-atk-api-tvarka-atk-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-tvarka-atk-api-api-openapi.yml
- filename: tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Tvarka ATK QES Signing API (paid Tier Addendum) API
  slug: tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api-openapi.yml
- filename: tvarka-atk-api-validation-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Validation API
  slug: tvarka-atk-api-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-validation-api-openapi.yml
- filename: tvarka-atk-api-well-known-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Well Known API
  slug: tvarka-atk-api-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/openapi/tvarka-atk-api-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:dmarc@tvarka.pro; ruf=mailto:dmarc@tvarka.pro; fo=1; adkim=r; aspf=r
  dnssec: false
  domain: tvarka.pro
  spf: false
hosts:
- cert_expires: Sep 18 13:31:31 2026 GMT
  host: atk.tvarka.pro
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  hsts_preload: false
  https: true
  role: api + developer portal
  tls_version: TLSv1.3
- cert_expires: Sep 18 13:31:31 2026 GMT
  host: tvarka.pro
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  hsts_preload: false
  https: true
  role: company site, terms, privacy, security, llms.txt
  tls_version: TLSv1.3
- cert_expires: Sep 18 13:31:31 2026 GMT
  host: sign.tvarka.pro
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  hsts_preload: false
  https: true
  role: pairing landing host referenced by AuthPairingHint.pairingUrl
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tvarka Atk Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tvarka ATK API, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Tvarka ATK API
provider_slug: tvarka-atk-api
slug: tvarka-atk-api-domain-security
source_filename: tvarka-atk-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI servers[] hosts\nprobed: '2026-08-09'\nhosts:\n  - host: atk.tvarka.pro\n    role: api + developer portal\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Sep 18 13:31:31 2026 GMT\n    hsts: true\n    hsts_max_age: 15552000\n    hsts_include_subdomains: true\n    hsts_preload: false\n  - host: tvarka.pro\n    role: company site, terms, privacy, security, llms.txt\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Sep 18 13:31:31 2026 GMT\n    hsts: true\n    hsts_max_age: 15552000\n    hsts_include_subdomains: true\n    hsts_preload: false\n  - host: sign.tvarka.pro\n    role: pairing landing host referenced by AuthPairingHint.pairingUrl\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Sep 18 13:31:31 2026 GMT\n    hsts: true\n    hsts_max_age: 15552000\n    hsts_include_subdomains: true\n    hsts_preload: false\ndomains:\n  - domain: tvarka.pro\n\
  \    dnssec: false\n    caa: []\n    spf: false\n    dmarc: true\n    dmarc_policy: quarantine\n    dmarc_record: >-\n      v=DMARC1; p=quarantine; rua=mailto:dmarc@tvarka.pro; ruf=mailto:dmarc@tvarka.pro; fo=1;\n      adkim=r; aspf=r\nnotes: >-\n  All three hosts sit behind Cloudflare (104.21.24.241 / 172.67.221.53) on one wildcard certificate,\n  TLS 1.3 with HSTS including subdomains on each. Gaps observed and recorded as absences, not\n  assumptions: no DNSSEC DS record, no CAA record set, and no SPF TXT record on tvarka.pro (DMARC is\n  published at p=quarantine with aggregate and forensic reporting, but without SPF it rests on DKIM\n  alignment alone). No /.well-known/security.txt on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvarka-atk-api/refs/heads/main/security/tvarka-atk-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Digital Signature
- eIDAS
- QES
- Lithuania
- OpenAPI
- eID
- Smart-ID
- Mobile-ID
- NFC
- Timestamping
- LTV
- Webhook
- Identity
- Trust Services
- GDPR
---
