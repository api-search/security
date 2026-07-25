---
api_specs:
- filename: authsignal-actions-api-openapi.yml
  format: yaml
  label: Authsignal Actions API
  slug: authsignal-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authsignal/refs/heads/main/openapi/authsignal-actions-api-openapi.yml
- filename: authsignal-authenticators-api-openapi.yml
  format: yaml
  label: Authsignal Authenticators API
  slug: authsignal-authenticators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authsignal/refs/heads/main/openapi/authsignal-authenticators-api-openapi.yml
- filename: authsignal-challenges-api-openapi.yml
  format: yaml
  label: Authsignal Challenges API
  slug: authsignal-challenges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authsignal/refs/heads/main/openapi/authsignal-challenges-api-openapi.yml
- filename: authsignal-devices-api-openapi.yml
  format: yaml
  label: Authsignal Devices API
  slug: authsignal-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authsignal/refs/heads/main/openapi/authsignal-devices-api-openapi.yml
- filename: authsignal-sessions-api-openapi.yml
  format: yaml
  label: Authsignal Sessions API
  slug: authsignal-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authsignal/refs/heads/main/openapi/authsignal-sessions-api-openapi.yml
- filename: authsignal-users-api-openapi.yml
  format: yaml
  label: Authsignal Users API
  slug: authsignal-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authsignal/refs/heads/main/openapi/authsignal-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: authsignal.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.authsignal.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 20:03:55 2026 GMT
  host: docs.authsignal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: api.authsignal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Authsignal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authsignal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Authsignal
provider_slug: authsignal
slug: authsignal-domain-security
source_filename: authsignal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.authsignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: docs.authsignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 20:03:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.authsignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: authsignal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authsignal/refs/heads/main/security/authsignal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Passkeys
- MFA
- Step-Up
- Passwordless
- Risk
- Biometrics
- Identity Verification
---
