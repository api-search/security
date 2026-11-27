---
api_specs:
- filename: bridgenode-cc-models-api-openapi.yml
  format: yaml
  label: BridgeNode Models API
  slug: bridgenode-cc-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bridgenode-cc/openapi/bridgenode-cc-models-api-openapi.yml
- filename: bridgenode-cc-chat-completions-api-openapi.yml
  format: yaml
  label: BridgeNode Chat Completions API
  slug: bridgenode-cc-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bridgenode-cc/openapi/bridgenode-cc-chat-completions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bridgenode.cc
  spf: false
hosts:
- cert_expires: Dec  7 17:27:39 2026 GMT
  host: bridgenode.cc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BridgeNode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BridgeNode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BridgeNode
provider_slug: bridgenode-cc
slug: bridgenode-cc-domain-security
source_filename: bridgenode-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bridgenode.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 17:27:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bridgenode.cc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bridgenode-cc/security/bridgenode-cc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Inference
- Payments
- Solana
- OpenAI-Compatible
---
