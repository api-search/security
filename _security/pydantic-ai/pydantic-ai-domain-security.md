---
api_specs:
- filename: pydantic-ai-discovery-openapi.yml
  format: yaml
  label: PydanticAI Agent Framework
  slug: pydantic-ai-agent-framework
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-discovery-openapi.yml
- filename: pydantic-ai-logfire-openapi.yml
  format: yaml
  label: Pydantic Logfire
  slug: pydantic-logfire
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/openapi/pydantic-ai-logfire-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pydantic.dev
  spf: true
hosts:
- cert_expires: Sep  4 17:29:51 2026 GMT
  host: pydantic.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 01:55:43 2026 GMT
  host: logfire.pydantic.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 14:56:07 2026 GMT
  host: logfire-us.pydantic.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pydantic Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PydanticAI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PydanticAI
provider_slug: pydantic-ai
slug: pydantic-ai-domain-security
source_filename: pydantic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pydantic.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 17:29:51 2026 GMT\n  hsts: false\n- host: logfire.pydantic.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 01:55:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: logfire-us.pydantic.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:56:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pydantic.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pydantic-ai/refs/heads/main/security/pydantic-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Agents
- Python
- LLM
- Type Safety
- Structured Outputs
- Dependency Injection
- OpenAI
- Anthropic
- Gemini
- Observability
- Framework
---
