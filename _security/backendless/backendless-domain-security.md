---
api_specs:
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Data Service API
  slug: data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless User Service API
  slug: users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless File Service API
  slug: files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Messaging and Push API
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Geo Service API
  slug: geo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Cache and Atomic Counters API
  slug: cache-counters
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
- filename: backendless-openapi.yml
  format: yaml
  label: Backendless Cloud Code API
  slug: cloud-code
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/openapi/backendless-openapi.yml
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issue "sectigo.com"
  - 128 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: backendless.com
  spf: true
hosts:
- cert_expires: Sep 26 01:27:46 2026 GMT
  host: backendless.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Backendless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Backendless, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Backendless
provider_slug: backendless
slug: backendless-domain-security
source_filename: backendless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backendless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 01:27:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: backendless.com\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issue \"sectigo.com\"\n  - 128 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backendless/refs/heads/main/security/backendless-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BaaS
- Backend as a Service
- Visual Development
- Low Code
- Database
- Realtime
---
