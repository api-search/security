---
api_specs:
- filename: writer-openapi.yml
  format: yaml
  label: Writer Chat Completion API
  slug: writer-chat-completion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Text Generation API
  slug: writer-text-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Tool Calling API
  slug: writer-tool-calling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Knowledge Graph API
  slug: writer-knowledge-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Files API
  slug: writer-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Applications API
  slug: writer-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Vision API
  slug: writer-vision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Web Search API
  slug: writer-web-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Translation API
  slug: writer-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Models API
  slug: writer-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer Guardrails API
  slug: writer-guardrails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
- filename: writer-openapi.yml
  format: yaml
  label: Writer API Keys API
  slug: writer-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/openapi/writer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: writer.com
  spf: true
hosts:
- cert_expires: Aug 13 00:20:15 2026 GMT
  host: writer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 05:11:07 2026 GMT
  host: dev.writer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 00:11:08 2026 GMT
  host: api.writer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Writer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Writer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Writer
provider_slug: writer
slug: writer-domain-security
source_filename: writer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: writer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 00:20:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.writer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:11:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.writer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 00:11:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: writer.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/writer/refs/heads/main/security/writer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- LLM
- Enterprise
- Content Generation
- Palmyra
- Agents
---
