---
api_specs:
- filename: softr-openapi.yml
  format: yaml
  label: Softr Users Management API
  slug: users-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/softr/refs/heads/main/openapi/softr-openapi.yml
- filename: softr-openapi.yml
  format: yaml
  label: Softr Database API
  slug: app-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/softr/refs/heads/main/openapi/softr-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: softr.io
  spf: true
hosts:
- cert_expires: Aug 11 20:40:17 2026 GMT
  host: www.softr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 03:33:15 2026 GMT
  host: docs.softr.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 20:40:17 2026 GMT
  host: studio-api.softr.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Softr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Softr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Softr
provider_slug: softr
slug: softr-domain-security
source_filename: softr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.softr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 20:40:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.softr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:33:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: studio-api.softr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 20:40:17 2026 GMT\n  hsts: null\ndomains:\n- domain: softr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/softr/refs/heads/main/security/softr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- No Code
- App Builder
- Client Portals
- User Management
- Database
---
