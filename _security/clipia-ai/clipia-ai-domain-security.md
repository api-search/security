---
api_specs:
- filename: clipia-ai-account-api-openapi.yml
  format: yaml
  label: Clipia.ai Account API
  slug: clipia-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-account-api-openapi.yml
- filename: clipia-ai-llm-api-openapi.yml
  format: yaml
  label: Clipia.ai LLM API
  slug: clipia-ai-llm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-llm-api-openapi.yml
- filename: clipia-ai-models-api-openapi.yml
  format: yaml
  label: Clipia.ai Models API
  slug: clipia-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-models-api-openapi.yml
- filename: clipia-ai-queue-api-openapi.yml
  format: yaml
  label: Clipia.ai Queue API
  slug: clipia-ai-queue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clipia-ai/openapi/clipia-ai-queue-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clipia.ai
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: clipia.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clipia.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clipia.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clipia.ai
provider_slug: clipia-ai
slug: clipia-ai-domain-security
source_filename: clipia-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clipia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clipia.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/clipia-ai/security/clipia-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Video Generation
- Image Generation
- Generative AI
- MCP
---
