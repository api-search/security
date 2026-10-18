---
api_specs:
- filename: libertai-aleph-credits-api-openapi.yml
  format: yaml
  label: LibertAI Aleph Credits API
  slug: libertai-aleph-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-aleph-credits-api-openapi.yml
- filename: libertai-auth-api-openapi.yml
  format: yaml
  label: LibertAI Auth API
  slug: libertai-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-auth-api-openapi.yml
- filename: libertai-health-api-openapi.yml
  format: yaml
  label: LibertAI Health API
  slug: libertai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-health-api-openapi.yml
- filename: libertai-models-api-openapi.yml
  format: yaml
  label: LibertAI Models API
  slug: libertai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-models-api-openapi.yml
- filename: libertai-proxy-api-openapi.yml
  format: yaml
  label: LibertAI Proxy API
  slug: libertai-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-proxy-api-openapi.yml
- filename: libertai-search-api-openapi.yml
  format: yaml
  label: LibertAI Search API
  slug: libertai-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/openapi/libertai-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: libertai.io
  spf: true
hosts:
- cert_expires: Jan  9 19:19:12 2027 GMT
  host: libertai.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Libertai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LibertAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LibertAI
provider_slug: libertai
slug: libertai-domain-security
source_filename: libertai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: libertai.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 19:19:12 2027 GMT\n  hsts: false\ndomains:\n- domain: libertai.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/libertai/refs/heads/main/security/libertai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Inference
- Model Routing
- OpenAI-Compatible
- Decentralized
- Confidential Computing
- x402
---
