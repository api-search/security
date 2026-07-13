---
api_specs:
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Users API
  slug: corbado-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Identifiers API
  slug: corbado-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Sessions API
  slug: corbado-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Passkeys API
  slug: corbado-passkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Connect Tokens API
  slug: corbado-connect-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
- filename: corbado-openapi.yml
  format: yaml
  label: Corbado Projects API
  slug: corbado-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/openapi/corbado-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: corbado.com
  spf: true
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: corbado.io
  spf: false
hosts:
- cert_expires: Aug 21 10:01:14 2026 GMT
  host: www.corbado.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 06:32:20 2026 GMT
  host: docs.corbado.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: backendapi.corbado.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corbado Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corbado, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Corbado
provider_slug: corbado
slug: corbado-domain-security
source_filename: corbado-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.corbado.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 10:01:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.corbado.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 06:32:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: backendapi.corbado.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: corbado.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: corbado.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corbado/refs/heads/main/security/corbado-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Passkeys
- WebAuthn
- Passwordless
- CIAM
- Identity
---
