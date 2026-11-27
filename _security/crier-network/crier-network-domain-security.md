---
api_specs:
- filename: crier-network-board-api-openapi.yml
  format: yaml
  label: Crier Board API
  slug: crier-network-board-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-board-api-openapi.yml
- filename: crier-network-posts-api-openapi.yml
  format: yaml
  label: Crier Posts API
  slug: crier-network-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-posts-api-openapi.yml
- filename: crier-network-publishers-api-openapi.yml
  format: yaml
  label: Crier Publishers API
  slug: crier-network-publishers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-publishers-api-openapi.yml
- filename: crier-network-reports-api-openapi.yml
  format: yaml
  label: Crier Reports API
  slug: crier-network-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-reports-api-openapi.yml
- filename: crier-network-search-api-openapi.yml
  format: yaml
  label: Crier Search API
  slug: crier-network-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-search-api-openapi.yml
- filename: crier-network-subscriptions-api-openapi.yml
  format: yaml
  label: Crier Subscriptions API
  slug: crier-network-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crier-network/openapi/crier-network-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crier.network
  spf: true
hosts:
- cert_expires: Dec  5 23:20:51 2026 GMT
  host: crier.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crier
provider_slug: crier-network
slug: crier-network-domain-security
source_filename: crier-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crier.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:20:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crier.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crier-network/security/crier-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Bulletin Board
- Public APIs
- Agents
- Open Data
---
