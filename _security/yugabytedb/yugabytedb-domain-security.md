---
api_specs:
- filename: yugabytedb-aeon-openapi.yml
  format: yaml
  label: YugabyteDB Aeon REST API
  slug: aeon
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabytedb/refs/heads/main/openapi/yugabytedb-aeon-openapi.yml
- filename: yugabytedb-anywhere-v1-universes.yaml
  format: yaml
  label: YugabyteDB Anywhere REST API
  slug: anywhere
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabytedb/refs/heads/main/openapi/yugabytedb-anywhere-v1-universes.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: yugabyte.com
  spf: true
hosts:
- cert_expires: Sep 25 19:15:11 2026 GMT
  host: www.yugabyte.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 07:23:46 2026 GMT
  host: docs.yugabyte.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 20:27:57 2026 GMT
  host: cloud.yugabyte.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yugabytedb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YugabyteDB, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: YugabyteDB
provider_slug: yugabytedb
slug: yugabytedb-domain-security
source_filename: yugabytedb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yugabyte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 19:15:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.yugabyte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 07:23:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.yugabyte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:27:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yugabyte.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yugabytedb/refs/heads/main/security/yugabytedb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Database
- Database
- DBaaS
- Distributed SQL
- PostgreSQL
---
