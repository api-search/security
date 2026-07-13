---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appwrite.io
  spf: true
hosts:
- cert_expires: Sep 28 01:59:01 2026 GMT
  host: appwrite.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 19:03:11 2026 GMT
  host: cloud.appwrite.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appwrite Graphql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appwrite GraphQL, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Appwrite GraphQL
provider_slug: appwrite-graphql
slug: appwrite-graphql-domain-security
source_filename: appwrite-graphql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appwrite.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 01:59:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.appwrite.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 19:03:11 2026 GMT\n  hsts: false\ndomains:\n- domain: appwrite.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appwrite-graphql/refs/heads/main/security/appwrite-graphql-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- Backend as a Service
- BaaS
- Database
- Authentication
- Storage
- Open Source
---
