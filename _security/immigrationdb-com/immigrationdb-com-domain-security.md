---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: immigrationdb.com
  spf: true
hosts:
- cert_expires: Feb  9 00:03:07 2027 GMT
  host: immigrationdb.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ImmigrationDB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ImmigrationDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ImmigrationDB
provider_slug: immigrationdb-com
slug: immigrationdb-com-domain-security
source_filename: immigrationdb-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: immigrationdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 00:03:07 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: immigrationdb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/immigrationdb-com/security/immigrationdb-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Migration
- Data
- Open Data
- Free
---
