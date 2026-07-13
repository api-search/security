---
api_specs:
- filename: turnkey-openapi.yml
  format: yaml
  label: Turnkey Organizations & Sub-Organizations API
  slug: turnkey-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/openapi/turnkey-openapi.yml
- filename: turnkey-openapi.yml
  format: yaml
  label: Turnkey Wallets API
  slug: turnkey-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/openapi/turnkey-openapi.yml
- filename: turnkey-openapi.yml
  format: yaml
  label: Turnkey Private Keys API
  slug: turnkey-private-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/openapi/turnkey-openapi.yml
- filename: turnkey-openapi.yml
  format: yaml
  label: Turnkey Signing & Activities API
  slug: turnkey-signing-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/openapi/turnkey-openapi.yml
- filename: turnkey-openapi.yml
  format: yaml
  label: Turnkey Users, Policies & Authenticators API
  slug: turnkey-users-policies-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/openapi/turnkey-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: turnkey.com
  spf: true
hosts:
- cert_expires: Oct  5 00:03:44 2026 GMT
  host: www.turnkey.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 12:48:10 2026 GMT
  host: docs.turnkey.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 17:48:20 2026 GMT
  host: api.turnkey.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Turnkey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Turnkey, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Turnkey
provider_slug: turnkey
slug: turnkey-domain-security
source_filename: turnkey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.turnkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.turnkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 12:48:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.turnkey.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 17:48:20 2026 GMT\n  hsts: null\ndomains:\n- domain: turnkey.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turnkey/refs/heads/main/security/turnkey-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Crypto
- Wallets
- Key Management
- Signing
- Secure Enclaves
---
