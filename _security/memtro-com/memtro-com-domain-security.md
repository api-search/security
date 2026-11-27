---
api_specs:
- filename: memtro-com-api-openapi.yml
  format: yaml
  label: Memtro API API
  slug: memtro-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memtro-com/openapi/_original/memtro-com-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: memtro.com
  spf: true
hosts:
- cert_expires: Jan 16 15:45:12 2027 GMT
  host: www.memtro.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Memtro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memtro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Memtro
provider_slug: memtro-com
slug: memtro-com-domain-security
source_filename: memtro-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.memtro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 15:45:12 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: memtro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/memtro-com/security/memtro-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Memory
- Connectors
- Data Integration
---
