---
api_specs:
- filename: stack-auth-openapi.yml
  format: yaml
  label: Stack Auth REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-auth/refs/heads/main/openapi/stack-auth-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stack-auth.com
  spf: true
hosts:
- cert_expires: Sep 23 08:41:10 2026 GMT
  host: stack-auth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 09:35:08 2026 GMT
  host: docs.stack-auth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 09:05:43 2026 GMT
  host: api.stack-auth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stack Auth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stack Auth, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stack Auth
provider_slug: stack-auth
slug: stack-auth-domain-security
source_filename: stack-auth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stack-auth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 08:41:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.stack-auth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 09:35:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.stack-auth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 09:05:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: stack-auth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-auth/refs/heads/main/security/stack-auth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- User Management
- Open Source
- Self-Hosted
- Identity
- Organizations
- RBAC
---
