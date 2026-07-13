---
api_specs:
- filename: ghost-admin-api-openapi.yml
  format: yaml
  label: Ghost Admin API
  slug: ghost-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-admin-api-openapi.yml
- filename: ghost-content-api-openapi.yml
  format: yaml
  label: Ghost Content API
  slug: ghost-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/openapi/ghost-content-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ghost.org
  spf: true
hosts:
- cert_expires: Sep 23 21:23:50 2026 GMT
  host: ghost.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:18:17 2026 GMT
  host: docs.ghost.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ghost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ghost, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ghost
provider_slug: ghost
slug: ghost-domain-security
source_filename: ghost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ghost.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:23:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ghost.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:18:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ghost.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ghost/refs/heads/main/security/ghost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Publishing
- Newsletters
- Memberships
- Content
- Open Source
---
