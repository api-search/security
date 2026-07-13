---
api_specs:
- filename: nhost-authentication-openapi.yml
  format: yaml
  label: Nhost Authentication API
  slug: nhost-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-authentication-openapi.yml
- filename: nhost-storage-openapi.yml
  format: yaml
  label: Nhost Storage API
  slug: nhost-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-storage-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nhost.io
  spf: true
hosts:
- cert_expires: Aug 10 05:56:32 2026 GMT
  host: nhost.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 12:38:19 2026 GMT
  host: docs.nhost.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nhost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nhost, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nhost
provider_slug: nhost
slug: nhost-domain-security
source_filename: nhost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nhost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 05:56:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.nhost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 12:38:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nhost.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/security/nhost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- PostgreSQL
- Authentication
- File Storage
- Serverless Functions
- Real-Time
- Open Source
- Firebase Alternative
- Backend as a Service
- BaaS
---
