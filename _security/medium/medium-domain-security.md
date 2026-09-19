---
api_specs:
- filename: medium-authorization-api-openapi.yml
  format: yaml
  label: medium Authorization API
  slug: medium-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-authorization-api-openapi.yml
- filename: medium-images-api-openapi.yml
  format: yaml
  label: medium Images API
  slug: medium-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-images-api-openapi.yml
- filename: medium-posts-api-openapi.yml
  format: yaml
  label: medium Posts API
  slug: medium-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-posts-api-openapi.yml
- filename: medium-publications-api-openapi.yml
  format: yaml
  label: medium Publications API
  slug: medium-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-publications-api-openapi.yml
- filename: medium-tokens-api-openapi.yml
  format: yaml
  label: medium Tokens API
  slug: medium-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-tokens-api-openapi.yml
- filename: medium-users-api-openapi.yml
  format: yaml
  label: medium Users API
  slug: medium-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/openapi/medium-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: medium.com
  spf: true
hosts:
- cert_expires: Dec  4 21:48:00 2026 GMT
  host: api.medium.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 21:48:00 2026 GMT
  host: medium.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Medium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medium, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Medium
provider_slug: medium
slug: medium-domain-security
source_filename: medium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.medium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 21:48:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: medium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 21:48:00 2026 GMT\n  hsts: null\ndomains:\n- domain: medium.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/security/medium-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Publishing
- Content
- Blogging
- Media
- Social
- Writing
- Authentication
- Deprecated API
---
