---
api_specs:
- filename: linkagi-model-api-anthropic-style-route-api-openapi.yml
  format: yaml
  label: LinkAGI Model API Anthropic-style route API
  slug: linkagi-model-api-anthropic-style-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/openapi/linkagi-model-api-anthropic-style-route-api-openapi.yml
- filename: linkagi-model-api-discovery-api-openapi.yml
  format: yaml
  label: LinkAGI Model API Discovery API
  slug: linkagi-model-api-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/openapi/linkagi-model-api-discovery-api-openapi.yml
- filename: linkagi-model-api-gemini-style-route-api-openapi.yml
  format: yaml
  label: LinkAGI Model API Gemini-style route API
  slug: linkagi-model-api-gemini-style-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/openapi/linkagi-model-api-gemini-style-route-api-openapi.yml
- filename: linkagi-model-api-openai-compatible-api-openapi.yml
  format: yaml
  label: LinkAGI Model API OpenAI compatible API
  slug: linkagi-model-api-openai-compatible-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/openapi/linkagi-model-api-openai-compatible-api-openapi.yml
- filename: linkagi-model-api-public-metadata-api-openapi.yml
  format: yaml
  label: LinkAGI Model API Public metadata API
  slug: linkagi-model-api-public-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/openapi/linkagi-model-api-public-metadata-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: linktoagi.com
  spf: true
hosts:
- cert_expires: Oct  8 05:19:27 2026 GMT
  host: docs.linktoagi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 05:19:27 2026 GMT
  host: api.linktoagi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linkagi Model Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LinkAGI Model API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LinkAGI Model API
provider_slug: linkagi-model-api
slug: linkagi-model-api-domain-security
source_filename: linkagi-model-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.linktoagi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:19:27 2026 GMT\n  hsts: false\n- host: api.linktoagi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:19:27 2026 GMT\n  hsts: false\ndomains:\n- domain: linktoagi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linkagi-model-api/refs/heads/main/security/linkagi-model-api-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- LLM
- AI API gateway
- relay
- OpenAI-compatible
- Anthropic-compatible
- Gemini-compatible
- developer tools
- CLI coding agents
- model routing
- China
---
