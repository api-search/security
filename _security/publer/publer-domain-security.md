---
api_specs:
- filename: publer-openapi.yml
  format: yaml
  label: Publer Posts & Scheduling API
  slug: posts-scheduling
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-openapi.yml
- filename: publer-openapi.yml
  format: yaml
  label: Publer Accounts API
  slug: accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-openapi.yml
- filename: publer-openapi.yml
  format: yaml
  label: Publer Workspaces API
  slug: workspaces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-openapi.yml
- filename: publer-openapi.yml
  format: yaml
  label: Publer Media API
  slug: media
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-openapi.yml
- filename: publer-openapi.yml
  format: yaml
  label: Publer Jobs API
  slug: jobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/openapi/publer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: publer.com
  spf: true
hosts:
- cert_expires: Sep 29 07:17:01 2026 GMT
  host: publer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 23:46:03 2026 GMT
  host: app.publer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Publer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Publer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Publer
provider_slug: publer
slug: publer-domain-security
source_filename: publer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: publer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 07:17:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.publer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:46:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: publer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/publer/refs/heads/main/security/publer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media
- Scheduling
- Publishing
- Content Management
- Marketing
---
