---
api_specs:
- filename: chain-love-ai-context-api-openapi.yml
  format: yaml
  label: Chain.Love AI Context API
  slug: chain-love-ai-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chain-love/openapi/chain-love-ai-context-api-openapi.yml
- filename: chain-love-discovery-api-openapi.yml
  format: yaml
  label: Chain.Love Discovery API
  slug: chain-love-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chain-love/openapi/chain-love-discovery-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chain.love
  spf: true
hosts:
- cert_expires: Dec 24 15:24:07 2026 GMT
  host: chain.love
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chain.Love Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chain.Love, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chain.Love
provider_slug: chain-love
slug: chain-love-domain-security
source_filename: chain-love-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chain.love\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 15:24:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chain.love\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chain-love/security/chain-love-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web3 Infrastructure
- RPC
- Indexing
- Oracle
- Bridge
- Developer Tools
- Marketplace
---
