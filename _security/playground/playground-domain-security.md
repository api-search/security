---
api_specs:
- filename: playground-auth-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Auth API
  slug: playground-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-auth-api-openapi.yml
- filename: playground-avatars-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Avatars API
  slug: playground-avatars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-avatars-api-openapi.yml
- filename: playground-comments-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Comments API
  slug: playground-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-comments-api-openapi.yml
- filename: playground-custom-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Custom API
  slug: playground-custom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-custom-api-openapi.yml
- filename: playground-posts-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Posts API
  slug: playground-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-posts-api-openapi.yml
- filename: playground-session-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Session API
  slug: playground-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-session-api-openapi.yml
- filename: playground-thumbnails-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Thumbnails API
  slug: playground-thumbnails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-thumbnails-api-openapi.yml
- filename: playground-users-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service Users API
  slug: playground-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-users-api-openapi.yml
- filename: playground-to-dos-api-openapi.yml
  format: yaml
  label: Playground API — Free Stateful Mock REST & GraphQL Service To Dos API
  slug: playground-to-dos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/openapi/playground-to-dos-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nileslabs.com
  spf: false
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vercel.app
  spf: true
hosts:
- cert_expires: Nov 21 08:31:49 2026 GMT
  host: playground.nileslabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 19:48:08 2026 GMT
  host: playground-api-backend.vercel.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Playground Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Playground API — Free Stateful Mock REST & GraphQL Service, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Playground API — Free Stateful Mock REST & GraphQL Service
provider_slug: playground
slug: playground-domain-security
source_filename: playground-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playground.nileslabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 08:31:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: playground-api-backend.vercel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 19:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nileslabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: vercel.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/playground/refs/heads/main/security/playground-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- Testing
- Mock API
- api-sandbox
- REST
- GraphQL
- E2E Testing
---
