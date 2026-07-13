---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:hostmaster@postgresql.org"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: postgresql.org
  spf: true
hosts:
- cert_expires: Aug 31 17:09:46 2026 GMT
  host: www.postgresql.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 22:09:19 2026 GMT
  host: jdbc.postgresql.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 22:09:19 2026 GMT
  host: odbc.postgresql.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postgres Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PostgreSQL, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: PostgreSQL
provider_slug: postgres
slug: postgres-domain-security
source_filename: postgres-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.postgresql.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 17:09:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: jdbc.postgresql.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:09:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: odbc.postgresql.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:09:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: postgresql.org\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:hostmaster@postgresql.org\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postgres/refs/heads/main/security/postgres-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Database
- Relational Database
- SQL
- Open Source
- PostgreSQL
- Object-Relational
- Data Storage
---
