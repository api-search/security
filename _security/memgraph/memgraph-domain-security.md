---
api_specs:
- filename: memgraph-monitoring-api-openapi.yml
  format: yaml
  label: Memgraph Monitoring API
  slug: memgraph-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memgraph/refs/heads/main/openapi/memgraph-monitoring-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: memgraph.com
  spf: true
hosts:
- cert_expires: Sep 19 22:20:27 2026 GMT
  host: memgraph.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Memgraph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Memgraph, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Memgraph
provider_slug: memgraph
slug: memgraph-domain-security
source_filename: memgraph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memgraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:20:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: memgraph.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memgraph/refs/heads/main/security/memgraph-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Graph Database
- In-Memory
- Cypher
- Bolt
- Real-Time
---
