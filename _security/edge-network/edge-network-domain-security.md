---
api_specs:
- filename: edge-network-assist-api-openapi.yml
  format: yaml
  label: Edge Network Assist API
  slug: edge-network-assist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-assist-api-openapi.yml
- filename: edge-network-cdn-api-openapi.yml
  format: yaml
  label: Edge Network CDN API
  slug: edge-network-cdn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-cdn-api-openapi.yml
- filename: edge-network-compute-api-openapi.yml
  format: yaml
  label: Edge Network Compute API
  slug: edge-network-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-compute-api-openapi.yml
- filename: edge-network-deploy-api-openapi.yml
  format: yaml
  label: Edge Network Deploy API
  slug: edge-network-deploy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-deploy-api-openapi.yml
- filename: edge-network-discovery-api-openapi.yml
  format: yaml
  label: Edge Network Discovery API
  slug: edge-network-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-discovery-api-openapi.yml
- filename: edge-network-dns-api-openapi.yml
  format: yaml
  label: Edge Network DNS API
  slug: edge-network-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-dns-api-openapi.yml
- filename: edge-network-projects-api-openapi.yml
  format: yaml
  label: Edge Network Projects API
  slug: edge-network-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-projects-api-openapi.yml
- filename: edge-network-shield-api-openapi.yml
  format: yaml
  label: Edge Network Shield API
  slug: edge-network-shield-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-shield-api-openapi.yml
- filename: edge-network-signup-api-openapi.yml
  format: yaml
  label: Edge Network Signup API
  slug: edge-network-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-signup-api-openapi.yml
- filename: edge-network-storage-api-openapi.yml
  format: yaml
  label: Edge Network Storage API
  slug: edge-network-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-storage-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: edge.network
  spf: true
hosts:
- cert_expires: Dec 27 19:48:10 2026 GMT
  host: edge.network
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Edge Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edge Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Edge Network
provider_slug: edge-network
slug: edge-network-domain-security
source_filename: edge-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edge.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 19:48:10 2026 GMT\n  hsts: false\ndomains:\n- domain: edge.network\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/edge-network/security/edge-network-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud
- CDN
- Compute
- Storage
- DNS
- Security
- Artificial Intelligence
---
