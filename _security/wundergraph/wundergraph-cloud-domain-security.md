---
api_specs:
- filename: wundergraph-analytics-api-openapi.yml
  format: yaml
  label: WunderGraph Analytics API
  slug: wundergraph-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-analytics-api-openapi.yml
- filename: wundergraph-api-keys-api-openapi.yml
  format: yaml
  label: WunderGraph API Keys API
  slug: wundergraph-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-api-keys-api-openapi.yml
- filename: wundergraph-feature-flags-api-openapi.yml
  format: yaml
  label: WunderGraph Feature Flags API
  slug: wundergraph-feature-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-feature-flags-api-openapi.yml
- filename: wundergraph-feature-subgraphs-api-openapi.yml
  format: yaml
  label: WunderGraph Feature Subgraphs API
  slug: wundergraph-feature-subgraphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-feature-subgraphs-api-openapi.yml
- filename: wundergraph-federated-graphs-api-openapi.yml
  format: yaml
  label: WunderGraph Federated Graphs API
  slug: wundergraph-federated-graphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-federated-graphs-api-openapi.yml
- filename: wundergraph-monographs-api-openapi.yml
  format: yaml
  label: WunderGraph Monographs API
  slug: wundergraph-monographs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-monographs-api-openapi.yml
- filename: wundergraph-namespaces-api-openapi.yml
  format: yaml
  label: WunderGraph Namespaces API
  slug: wundergraph-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-namespaces-api-openapi.yml
- filename: wundergraph-router-api-openapi.yml
  format: yaml
  label: WunderGraph Router API
  slug: wundergraph-router-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-router-api-openapi.yml
- filename: wundergraph-schema-contracts-api-openapi.yml
  format: yaml
  label: WunderGraph Schema Contracts API
  slug: wundergraph-schema-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-schema-contracts-api-openapi.yml
- filename: wundergraph-subgraphs-api-openapi.yml
  format: yaml
  label: WunderGraph Subgraphs API
  slug: wundergraph-subgraphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/openapi/wundergraph-subgraphs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wundergraph.com
  spf: true
hosts:
- cert_expires: Aug 24 10:40:42 2026 GMT
  host: wundergraph.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 20:38:55 2026 GMT
  host: cosmo-docs.wundergraph.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 15:35:52 2026 GMT
  host: cosmo-cp.wundergraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wundergraph Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WunderGraph, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WunderGraph
provider_slug: wundergraph
slug: wundergraph-cloud-domain-security
source_filename: wundergraph-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wundergraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:40:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cosmo-docs.wundergraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:38:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: cosmo-cp.wundergraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:35:52 2026 GMT\n  hsts: null\ndomains:\n- domain: wundergraph.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wundergraph/refs/heads/main/security/wundergraph-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Federation
- GraphQL
- Management
- Schema Registry
- API Gateway
- Observability
- Agents
- Developer Tools
---
