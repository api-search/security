---
api_specs:
- filename: hey-api-get-api-openapi.yml
  format: yaml
  label: Hey API Get API
  slug: hey-api-get-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-get-api-openapi.yml
- filename: hey-api-hey-api-api-openapi.yml
  format: yaml
  label: Hey API Hey API API
  slug: hey-api-hey-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-hey-api-api-openapi.yml
- filename: hey-api-internal-api-openapi.yml
  format: yaml
  label: Hey API Internal API
  slug: hey-api-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-internal-api-openapi.yml
- filename: hey-api-organizations-api-openapi.yml
  format: yaml
  label: Hey API Organizations API
  slug: hey-api-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-organizations-api-openapi.yml
- filename: hey-api-specifications-api-openapi.yml
  format: yaml
  label: Hey API Specifications API
  slug: hey-api-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-specifications-api-openapi.yml
- filename: hey-api-users-api-openapi.yml
  format: yaml
  label: Hey API Users API
  slug: hey-api-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/openapi/hey-api-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: heyapi.dev
  spf: true
hosts:
- cert_expires: Sep 27 00:13:28 2026 GMT
  host: heyapi.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 12:52:40 2026 GMT
  host: api.heyapi.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hey Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hey API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hey API
provider_slug: hey-api
slug: hey-api-domain-security
source_filename: hey-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heyapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:13:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.heyapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:52:40 2026 GMT\n  hsts: false\ndomains:\n- domain: heyapi.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hey-api/refs/heads/main/security/hey-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Code Generation
- Developer Tools
- OpenAPI
- SDK
- TypeScript
- Python
- API Design
- Specifications
- Registry
- Open-Source
---
