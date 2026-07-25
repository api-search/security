---
api_specs:
- filename: instantdb-asyncapi.yml
  format: yaml
  label: InstantDB Realtime Sync API
  slug: instantdb-realtime-sync-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/asyncapi/instantdb-asyncapi.yml
- filename: instantdb-auth-api-openapi.yml
  format: yaml
  label: InstantDB Auth API
  slug: instantdb-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-auth-api-openapi.yml
- filename: instantdb-presence-api-openapi.yml
  format: yaml
  label: InstantDB Presence API
  slug: instantdb-presence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-presence-api-openapi.yml
- filename: instantdb-query-api-openapi.yml
  format: yaml
  label: InstantDB Query API
  slug: instantdb-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-query-api-openapi.yml
- filename: instantdb-storage-api-openapi.yml
  format: yaml
  label: InstantDB Storage API
  slug: instantdb-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-storage-api-openapi.yml
- filename: instantdb-transactions-api-openapi.yml
  format: yaml
  label: InstantDB Transactions API
  slug: instantdb-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/openapi/instantdb-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: instantdb.com
  spf: true
hosts:
- cert_expires: Sep 28 09:53:00 2026 GMT
  host: www.instantdb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: api.instantdb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instantdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InstantDB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InstantDB
provider_slug: instantdb
slug: instantdb-domain-security
source_filename: instantdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.instantdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 09:53:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.instantdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: instantdb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instantdb/refs/heads/main/security/instantdb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Realtime
- Sync
- Backend
- Local First
---
