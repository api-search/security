---
api_specs:
- filename: client-libraries
  format: yaml
  label: SpiceDB Permissions API
  slug: spicedb-permissions-api
  spec_type: OpenAPI
  url: https://authzed.com/docs/spicedb/getting-started/client-libraries
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: authzed.com
  spf: true
hosts:
- cert_expires: Oct  1 07:09:15 2026 GMT
  host: authzed.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 17:42:15 2026 GMT
  host: grpc.authzed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 05:46:25 2026 GMT
  host: app.authzed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Authzed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authzed, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Authzed
provider_slug: authzed
slug: authzed-domain-security
source_filename: authzed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: authzed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:09:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: grpc.authzed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 17:42:15 2026 GMT\n  hsts: null\n- host: app.authzed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 05:46:25 2026 GMT\n  hsts: null\ndomains:\n- domain: authzed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authzed/refs/heads/main/security/authzed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authorization
- Access Control
- Permissions
- Zanzibar
- SpiceDB
- gRPC
- REST
- Relationship-Based Access Control
- ReBAC
- Fine-Grained Authorization
- Identity
- Security
---
