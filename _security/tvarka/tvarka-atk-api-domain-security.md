---
api_specs:
- filename: tvarka-atk-api-auth-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Auth API
  slug: tvarka-atk-api-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-auth-api-openapi.yml
- filename: tvarka-atk-api-erasure-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Erasure API
  slug: tvarka-atk-api-erasure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-erasure-api-openapi.yml
- filename: tvarka-atk-api-ltv-api-openapi.yml
  format: yaml
  label: Tvarka ATK API LTV API
  slug: tvarka-atk-api-ltv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-ltv-api-openapi.yml
- filename: tvarka-atk-api-pairing-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Pairing API
  slug: tvarka-atk-api-pairing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-pairing-api-openapi.yml
- filename: tvarka-atk-api-sign-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Sign API
  slug: tvarka-atk-api-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-sign-api-openapi.yml
- filename: auth.json
  format: json
  label: Tvarka ATK API Tvarka ATK API API
  slug: tvarka-atk-api-tvarka-atk-api-api
  spec_type: Postman
  url: https://atk.tvarka.pro/postman/auth.json
- filename: auth.json
  format: json
  label: Tvarka ATK API Tvarka ATK QES Signing API (paid Tier Addendum) API
  slug: tvarka-atk-api-tvarka-atk-qes-signing-api-paid-tier-addendum-api
  spec_type: Postman
  url: https://atk.tvarka.pro/postman/auth.json
- filename: tvarka-atk-api-validation-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Validation API
  slug: tvarka-atk-api-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-validation-api-openapi.yml
- filename: tvarka-atk-api-well-known-api-openapi.yml
  format: yaml
  label: Tvarka ATK API Well Known API
  slug: tvarka-atk-api-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-atk-api-well-known-api-openapi.yml
- filename: tvarka-sign-api-openapi.yml
  format: yaml
  label: Tvarka Sign API
  slug: tvarka-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/openapi/tvarka-sign-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dmarc_record: v=DMARC1; p=quarantine; rua=mailto:dmarc@tvarka.pro; ruf=mailto:dmarc@tvarka.pro; fo=1; adkim=r; aspf=r
  dnssec: false
  dnssec_note: No DS record is published at the parent, so the zone is not DNSSEC-signed.
  domain: tvarka.pro
  spf: true
  spf_record: v=spf1 include:_spf.purelymail.com ~all
hosts:
- cert_expires: Nov 16 12:50:18 2026 GMT
  cert_issuer: Let's Encrypt (CN=YE2)
  edge: cloudflare
  host: atk.tvarka.pro
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  role: ATK API + developer portal
  tls_version: TLSv1.3
- cert_expires: Nov 16 12:50:18 2026 GMT
  cert_issuer: Let's Encrypt (CN=YE2)
  edge: cloudflare
  host: tvarka.pro
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  role: company site, terms, privacy, security page, security.txt, llms.txt
  tls_version: TLSv1.3
- cert_expires: Nov 16 12:50:18 2026 GMT
  cert_issuer: Let's Encrypt (CN=YE2)
  edge: cloudflare
  host: sign-api.tvarka.pro
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  role: Tvarka Sign API + MCP server (first probed 2026-08-31)
  tls_version: TLSv1.3
- cert_expires: Nov 16 12:50:18 2026 GMT
  cert_issuer: Let's Encrypt (CN=YE2)
  edge: cloudflare
  host: sign.tvarka.pro
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  role: pairing landing host referenced by AuthPairingHint.pairingUrl
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tvarka Atk Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tvarka ATK API, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tvarka ATK API
provider_slug: tvarka
slug: tvarka-atk-api-domain-security
source_filename: tvarka-atk-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI servers[] hosts\nprobed: '2026-08-31'\nprevious_probe: '2026-08-09'\nhosts:\n  - host: atk.tvarka.pro\n    role: ATK API + developer portal\n    https: true\n    tls_version: TLSv1.3\n    cert_issuer: \"Let's Encrypt (CN=YE2)\"\n    cert_expires: Nov 16 12:50:18 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: true\n    hsts_preload: false\n    edge: cloudflare\n  - host: tvarka.pro\n    role: company site, terms, privacy, security page, security.txt, llms.txt\n    https: true\n    tls_version: TLSv1.3\n    cert_issuer: \"Let's Encrypt (CN=YE2)\"\n    cert_expires: Nov 16 12:50:18 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: true\n    hsts_preload: false\n    edge: cloudflare\n  - host: sign-api.tvarka.pro\n    role: Tvarka Sign API + MCP server (first probed 2026-08-31)\n    https: true\n    tls_version: TLSv1.3\n\
  \    cert_issuer: \"Let's Encrypt (CN=YE2)\"\n    cert_expires: Nov 16 12:50:18 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: true\n    hsts_preload: false\n    edge: cloudflare\n  - host: sign.tvarka.pro\n    role: pairing landing host referenced by AuthPairingHint.pairingUrl\n    https: true\n    tls_version: TLSv1.3\n    cert_issuer: \"Let's Encrypt (CN=YE2)\"\n    cert_expires: Nov 16 12:50:18 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: true\n    hsts_preload: false\n    edge: cloudflare\ndomains:\n  - domain: tvarka.pro\n    dnssec: false\n    dnssec_note: No DS record is published at the parent, so the zone is not DNSSEC-signed.\n    caa:\n      - 0 issue \"comodoca.com\"\n      - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n      - 0 issue \"letsencrypt.org\"\n      - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n      - 0 issue \"sectigo.com\"\n      - 0 issue \"ssl.com\"\n      - 0 issuewild \"\
  comodoca.com\"\n      - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n      - 0 issuewild \"letsencrypt.org\"\n      - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n      - 0 issuewild \"sectigo.com\"\n      - 0 issuewild \"ssl.com\"\n    spf: true\n    spf_record: v=spf1 include:_spf.purelymail.com ~all\n    dmarc: true\n    dmarc_policy: quarantine\n    dmarc_record: 'v=DMARC1; p=quarantine; rua=mailto:dmarc@tvarka.pro; ruf=mailto:dmarc@tvarka.pro; fo=1; adkim=r; aspf=r'\ntxt_records_of_note:\n  - record: 'v=MCPv1; k=ed25519; p=<ed25519 public key>'\n    zone: tvarka.pro\n    kind: MCP server identity\n    note: >-\n      An MCPv1 DNS TXT record publishing an ed25519 public key at the apex. Found 2026-08-31; it was\n      not present, or not looked for, on 2026-08-09. It sits alongside the live MCP server at\n      https://sign-api.tvarka.pro/mcp, so this is a DNS-level identity claim for that server rather\n      than a stray record. Key value not reproduced here - it\
  \ is a public key, but there is no reason\n      to mirror it and every reason to read it from DNS at verification time.\n  - record: purelymail_ownership_proof=...\n    zone: tvarka.pro\n    kind: mail-provider domain verification\nposture:\n  strengths:\n    - HSTS with a one-year max-age and includeSubDomains on every host in the estate.\n    - TLS 1.3 everywhere, single wildcard-style certificate across all four hosts.\n    - CAA published, restricting issuance to six named CAs for both exact and wildcard names.\n    - SPF and DMARC published, DMARC at p=quarantine with both aggregate and forensic reporting.\n  gaps:\n    - No DNSSEC.\n    - HSTS is not preloaded.\n    - DMARC is p=quarantine rather than p=reject.\nchanges_since_previous_probe:\n  - Certificates renewed - expiry moved from Sep 18 2026 to Nov 16 2026.\n  - >-\n    HSTS max-age raised from 15552000 (180 days) to 31536000 (1 year) on every host, still with\n    includeSubDomains.\n  - New host in the estate - sign-api.tvarka.pro,\
  \ with the same posture as the rest.\n  - An MCPv1 DNS TXT identity record is now published at the tvarka.pro apex.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvarka/refs/heads/main/security/tvarka-atk-api-domain-security.yml
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
