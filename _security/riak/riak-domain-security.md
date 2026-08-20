---
api_specs:
- filename: riak-mapred-api-openapi.yml
  format: yaml
  label: Riak KV Mapred API
  slug: riak-mapred-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riak/refs/heads/main/openapi/riak-mapred-api-openapi.yml
- filename: riak-ping-api-openapi.yml
  format: yaml
  label: Riak KV Ping API
  slug: riak-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riak/refs/heads/main/openapi/riak-ping-api-openapi.yml
- filename: riak-riak-kv-http-api-api-openapi.yml
  format: yaml
  label: Riak KV Riak KV HTTP API API
  slug: riak-riak-kv-http-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riak/refs/heads/main/openapi/riak-riak-kv-http-api-api-openapi.yml
- filename: riak-search-api-openapi.yml
  format: yaml
  label: Riak KV Search API
  slug: riak-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riak/refs/heads/main/openapi/riak-search-api-openapi.yml
- filename: riak-stats-api-openapi.yml
  format: yaml
  label: Riak KV Stats API
  slug: riak-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riak/refs/heads/main/openapi/riak-stats-api-openapi.yml
- filename: riak-types-api-openapi.yml
  format: yaml
  label: Riak KV Types API
  slug: riak-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/riak/refs/heads/main/openapi/riak-types-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: riak.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: riak.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: docs.riak.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Riak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riak KV, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Riak KV
provider_slug: riak
slug: riak-domain-security
source_filename: riak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: riak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.riak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: riak.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riak/refs/heads/main/security/riak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- NoSQL
- Key-Value Store
- Distributed Systems
- Open-Source
- Basho
- CRDT
---
