---
api_specs:
- filename: databend-openapi-generated.yml
  format: yaml
  label: Databend API
  slug: databend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databend/openapi/_ae-authored/databend-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: databend.com
  spf: true
hosts:
- cert_expires: Jan 18 02:00:09 2027 GMT
  host: databend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Databend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Databend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Databend
provider_slug: databend
slug: databend-domain-security
source_filename: databend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: databend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 02:00:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: databend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/databend/security/databend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Warehouse
- Cloud
- Open Source
- Analytics
---
