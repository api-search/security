---
api_specs:
- filename: ydb-openapi-generated.yml
  format: yaml
  label: YDB API
  slug: ydb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ydb/openapi/_ae-authored/ydb-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ydb.tech
  spf: true
hosts:
- cert_expires: Feb 11 13:49:28 2027 GMT
  host: ydb.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: YDB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: YDB
provider_slug: ydb
slug: ydb-domain-security
source_filename: ydb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ydb.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 13:49:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ydb.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ydb/security/ydb-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Database
- Distributed
- SQL
- Open Source
- Cloud
---
