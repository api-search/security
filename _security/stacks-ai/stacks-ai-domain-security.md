---
api_specs:
- filename: stacks-ai-analytics-api-openapi.yml
  format: yaml
  label: Stacks Ai analytics API
  slug: stacks-ai-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/openapi/stacks-ai-analytics-api-openapi.yml
- filename: stacks-ai-knowledge-base-resources-api-openapi.yml
  format: yaml
  label: Stacks Ai Knowledge Base Resources API
  slug: stacks-ai-knowledge-base-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/openapi/stacks-ai-knowledge-base-resources-api-openapi.yml
- filename: stacks-ai-knowledge-base-sync-api-openapi.yml
  format: yaml
  label: Stacks Ai Knowledge Base Sync API
  slug: stacks-ai-knowledge-base-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/openapi/stacks-ai-knowledge-base-sync-api-openapi.yml
- filename: stacks-ai-knowledge-bases-api-openapi.yml
  format: yaml
  label: Stacks Ai Knowledge Bases API
  slug: stacks-ai-knowledge-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/openapi/stacks-ai-knowledge-bases-api-openapi.yml
- filename: stacks-ai-run-flow-api-openapi.yml
  format: yaml
  label: Stacks Ai Run Flow API
  slug: stacks-ai-run-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/openapi/stacks-ai-run-flow-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stackai.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stack-ai.com
  spf: true
hosts:
- cert_expires: Oct  1 00:57:01 2026 GMT
  host: docs.stackai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  6 16:56:56 2026 GMT
  host: api.stack-ai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: stack-inference.com
  https: false
kind: domain-security
layout: security
method: probed
name: Stacks Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stacks Ai, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stacks Ai
provider_slug: stacks-ai
slug: stacks-ai-domain-security
source_filename: stacks-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.stackai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 00:57:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stack-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 16:56:56 2026 GMT\n  hsts: null\n- host: stack-inference.com\n  https: false\ndomains:\n- domain: stackai.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: stack-ai.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stacks-ai/refs/heads/main/security/stacks-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Agents
- LLM
- No-Code
- Automation
- Workflows
- RAG
- Knowledge Base
- Enterprise
---
