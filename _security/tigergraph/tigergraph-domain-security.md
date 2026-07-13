---
api_specs:
- filename: tigergraph-openapi.yml
  format: yaml
  label: TigerGraph REST++ Data API (Vertices & Edges)
  slug: tigergraph-restpp-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-openapi.yml
- filename: tigergraph-openapi.yml
  format: yaml
  label: TigerGraph Query API (Run GSQL Queries)
  slug: tigergraph-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-openapi.yml
- filename: tigergraph-openapi.yml
  format: yaml
  label: TigerGraph Schema API
  slug: tigergraph-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-openapi.yml
- filename: tigergraph-openapi.yml
  format: yaml
  label: TigerGraph Auth & Tokens API
  slug: tigergraph-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-openapi.yml
- filename: tigergraph-openapi.yml
  format: yaml
  label: TigerGraph Savanna (Cloud) API
  slug: tigergraph-savanna-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/openapi/tigergraph-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tigergraph.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tgcloud.io
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.tigergraph.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 10:01:35 2026 GMT
  host: docs.tigergraph.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: <workspace-id>.i.tgcloud.io
  https: false
kind: domain-security
layout: security
method: probed
name: Tigergraph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TigerGraph, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TigerGraph
provider_slug: tigergraph
slug: tigergraph-domain-security
source_filename: tigergraph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tigergraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\n- host: docs.tigergraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 10:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: <workspace-id>.i.tgcloud.io\n  https: false\ndomains:\n- domain: tigergraph.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tgcloud.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigergraph/refs/heads/main/security/tigergraph-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Graph Database
- Analytics
- GSQL
- REST++
- Graph Analytics
---
