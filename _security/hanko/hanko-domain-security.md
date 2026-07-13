---
api_specs:
- filename: openapi-public.yaml
  format: yaml
  label: Hanko Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://docs.hanko.io/openapi-public.yaml
- filename: openapi-admin.yaml
  format: yaml
  label: Hanko Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://docs.hanko.io/openapi-admin.yaml
- filename: openapi-passkeys.yaml
  format: yaml
  label: Hanko Passkey API
  slug: passkey-api
  spec_type: OpenAPI
  url: https://docs.hanko.io/openapi-passkeys.yaml
- filename: openapi-flow.yaml
  format: yaml
  label: Hanko Flow API
  slug: flow-api
  spec_type: OpenAPI
  url: https://docs.hanko.io/openapi-flow.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hanko.io
  spf: true
hosts:
- cert_expires: Sep 11 21:14:28 2026 GMT
  host: www.hanko.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 04:14:00 2026 GMT
  host: docs.hanko.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 01:45:11 2026 GMT
  host: passkeys.hanko.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hanko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hanko, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hanko
provider_slug: hanko
slug: hanko-domain-security
source_filename: hanko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hanko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 21:14:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.hanko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:14:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: passkeys.hanko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:45:11 2026 GMT\n  hsts: null\ndomains:\n- domain: hanko.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hanko/refs/heads/main/security/hanko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Passkeys
- WebAuthn
- FIDO2
- Identity
- OAuth
- SAML
- Passwordless
- Open Source
---
