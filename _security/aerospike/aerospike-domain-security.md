---
api_specs:
- filename: aerospike-openapi.yml
  format: yaml
  label: Aerospike REST Gateway
  slug: rest-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerospike/refs/heads/main/openapi/aerospike-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aerospike.com
  spf: true
hosts:
- cert_expires: Sep 13 16:24:40 2026 GMT
  host: aerospike.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aerospike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aerospike, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aerospike
provider_slug: aerospike
slug: aerospike-domain-security
source_filename: aerospike-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aerospike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:24:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aerospike.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerospike/refs/heads/main/security/aerospike-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- NoSQL
- Real-Time
- Key-Value
- In-Memory
- Vector Database
- High Performance
---
