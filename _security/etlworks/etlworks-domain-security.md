---
api_specs:
- filename: etlworks-openapi-generated.yml
  format: yaml
  label: Etlworks API
  slug: etlworks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etlworks/openapi/_ae-authored/etlworks-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: etlworks.com
  spf: true
hosts:
- cert_expires: Jan  9 23:33:03 2027 GMT
  host: etlworks.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Etlworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Etlworks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Etlworks
provider_slug: etlworks
slug: etlworks-domain-security
source_filename: etlworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: etlworks.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 23:33:03 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: etlworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/etlworks/security/etlworks-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Data Integration
- ETL
- API
- Cloud
---
