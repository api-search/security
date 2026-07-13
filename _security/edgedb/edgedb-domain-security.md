---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geldata.com
  spf: true
hosts:
- cert_expires: Sep 12 08:27:32 2026 GMT
  host: www.geldata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 11:23:04 2026 GMT
  host: docs.geldata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 22:38:19 2026 GMT
  host: cloud.geldata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edgedb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EdgeDB, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EdgeDB
provider_slug: edgedb
slug: edgedb-domain-security
source_filename: edgedb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 08:27:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.geldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:23:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cloud.geldata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:38:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: geldata.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edgedb/refs/heads/main/security/edgedb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- PostgreSQL
- Graph Database
- Object-Relational
- EdgeQL
- GraphQL
- HTTP API
- Cloud Database
---
