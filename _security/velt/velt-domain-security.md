---
api_specs:
- filename: velt-openapi.yml
  format: yaml
  label: Velt Comments API
  slug: velt-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Users API
  slug: velt-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Organizations API
  slug: velt-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Documents API
  slug: velt-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Notifications API
  slug: velt-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Webhooks API
  slug: velt-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
- filename: velt-openapi.yml
  format: yaml
  label: Velt Auth Tokens API
  slug: velt-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/openapi/velt-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: velt.dev
  spf: true
hosts:
- cert_expires: Aug 12 19:55:30 2026 GMT
  host: velt.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 00:57:33 2026 GMT
  host: api.velt.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Velt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Velt, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Velt
provider_slug: velt
slug: velt-domain-security
source_filename: velt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: velt.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 19:55:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.velt.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:57:33 2026 GMT\n  hsts: null\ndomains:\n- domain: velt.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velt/refs/heads/main/security/velt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real-Time Collaboration
- Comments
- Presence
- Notifications
- SDK
- Webhooks
---
