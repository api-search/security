---
api_specs:
- filename: anthropic-messages-api-openapi.yml
  format: yaml
  label: Anthropic Messages API
  slug: anthropic-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-messages-api-openapi.yml
- filename: anthropic-models-api-openapi.yml
  format: yaml
  label: Anthropic Models API
  slug: anthropic-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-models-api-openapi.yml
- filename: anthropic-message-batches-api-openapi.yml
  format: yaml
  label: Anthropic Message Batches API
  slug: anthropic-message-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-message-batches-api-openapi.yml
- filename: anthropic-files-api-openapi.yml
  format: yaml
  label: Anthropic Files API
  slug: anthropic-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-files-api-openapi.yml
- filename: anthropic-admin-api-openapi.yml
  format: yaml
  label: Anthropic Admin API
  slug: anthropic-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-admin-api-openapi.yml
- filename: anthropic-prompts-api-openapi.yml
  format: yaml
  label: Anthropic Prompts API
  slug: anthropic-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-prompts-api-openapi.yml
- filename: anthropic-token-counting-api-openapi.yml
  format: yaml
  label: Anthropic Token Counting API
  slug: anthropic-token-counting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-token-counting-api-openapi.yml
- filename: anthropic-skills-api-openapi.yml
  format: yaml
  label: Anthropic Skills API
  slug: anthropic-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-skills-api-openapi.yml
- filename: anthropic-usage-cost-api-openapi.yml
  format: yaml
  label: Anthropic Usage and Cost API
  slug: anthropic-usage-cost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-usage-cost-api-openapi.yml
- filename: anthropic-claude-code-analytics-api-openapi.yml
  format: yaml
  label: Anthropic Claude Code Analytics API
  slug: anthropic-claude-code-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-claude-code-analytics-api-openapi.yml
- filename: anthropic-managed-agents-api-openapi.yml
  format: yaml
  label: Anthropic Managed Agents API
  slug: anthropic-managed-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/openapi/anthropic-managed-agents-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: claude.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anthropic.com
  spf: true
hosts:
- cert_expires: Sep 24 00:48:33 2026 GMT
  host: platform.claude.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 15:03:46 2026 GMT
  host: www.anthropic.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 19:48:08 2026 GMT
  host: docs.anthropic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anthropic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anthropic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Anthropic
provider_slug: anthropic
slug: anthropic-domain-security
source_filename: anthropic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: platform.claude.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 00:48:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.anthropic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: docs.anthropic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: claude.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: anthropic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anthropic/refs/heads/main/security/anthropic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Claude
- Foundation Models
- Large Language Models
- Machine Learning
- MCP
- Agents
---
