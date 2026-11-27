---
api_specs:
- filename: opentsdb-openapi-generated.yml
  format: yaml
  label: OpenTSDB API
  slug: opentsdb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentsdb/openapi/_ae-authored/opentsdb-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opentsdb.net
  spf: false
hosts:
- cert_expires: Jan 19 19:28:21 2027 GMT
  host: opentsdb.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenTSDB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenTSDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenTSDB
provider_slug: opentsdb
slug: opentsdb-domain-security
source_filename: opentsdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opentsdb.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 19:28:21 2027 GMT\n  hsts: false\ndomains:\n- domain: opentsdb.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/opentsdb/security/opentsdb-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Time Series
- Monitoring
- Open Source
- Database
---
