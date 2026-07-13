---
api_specs:
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Admin Members API
  slug: circle-community-admin-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Admin Spaces API
  slug: circle-community-admin-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Admin Posts and Comments API
  slug: circle-community-admin-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Admin Events API
  slug: circle-community-admin-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Admin Courses API
  slug: circle-community-admin-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Headless Member API
  slug: circle-community-headless-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Headless Auth API
  slug: circle-community-headless-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-asyncapi.yml
  format: yaml
  label: Circle Realtime WebSocket API
  slug: circle-community-realtime-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/asyncapi/circle-community-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: circle.so
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: circle.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 19:55:49 2026 GMT
  host: api.circle.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: app.circle.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Circle Community Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Circle
provider_slug: circle-community
slug: circle-community-domain-security
source_filename: circle-community-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: circle.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.circle.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:55:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.circle.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: circle.so\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/security/circle-community-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Community
- Creators
- Courses
- Memberships
- Events
- Chat
- Community Platform
---
