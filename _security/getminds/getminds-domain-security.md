---
api_specs:
- filename: getminds-agent-runs-api-openapi.yml
  format: yaml
  label: Minds Agent Runs API
  slug: getminds-agent-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-agent-runs-api-openapi.yml
- filename: getminds-api-keys-api-openapi.yml
  format: yaml
  label: Minds API Keys API
  slug: getminds-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-api-keys-api-openapi.yml
- filename: getminds-audiences-api-openapi.yml
  format: yaml
  label: Minds Audiences API
  slug: getminds-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-audiences-api-openapi.yml
- filename: getminds-auth-api-openapi.yml
  format: yaml
  label: Minds Auth API
  slug: getminds-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-auth-api-openapi.yml
- filename: getminds-chat-api-openapi.yml
  format: yaml
  label: Minds Chat API
  slug: getminds-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-chat-api-openapi.yml
- filename: getminds-knowledge-api-openapi.yml
  format: yaml
  label: Minds Knowledge API
  slug: getminds-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-knowledge-api-openapi.yml
- filename: getminds-meta-api-openapi.yml
  format: yaml
  label: Minds Meta API
  slug: getminds-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-meta-api-openapi.yml
- filename: getminds-minds-api-openapi.yml
  format: yaml
  label: Minds Minds API
  slug: getminds-minds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-minds-api-openapi.yml
- filename: getminds-models-api-openapi.yml
  format: yaml
  label: Minds Models API
  slug: getminds-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-models-api-openapi.yml
- filename: getminds-research-api-openapi.yml
  format: yaml
  label: Minds Research API
  slug: getminds-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-research-api-openapi.yml
- filename: getminds-studies-api-openapi.yml
  format: yaml
  label: Minds Studies API
  slug: getminds-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-studies-api-openapi.yml
- filename: getminds-study-drafts-api-openapi.yml
  format: yaml
  label: Minds Study Drafts API
  slug: getminds-study-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-study-drafts-api-openapi.yml
- filename: getminds-study-runs-api-openapi.yml
  format: yaml
  label: Minds Study Runs API
  slug: getminds-study-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-study-runs-api-openapi.yml
- filename: getminds-study-templates-api-openapi.yml
  format: yaml
  label: Minds Study Templates API
  slug: getminds-study-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/openapi/getminds-study-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getminds.ai
  spf: true
hosts:
- cert_expires: Dec  7 08:26:13 2026 GMT
  host: getminds.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 08:26:13 2026 GMT
  host: api.getminds.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Getminds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Minds, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Minds
provider_slug: getminds
slug: getminds-domain-security
source_filename: getminds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getminds.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 08:26:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.getminds.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 08:26:13 2026 GMT\n  hsts: false\ndomains:\n- domain: getminds.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getminds/refs/heads/main/security/getminds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Synthetic Research
- Market Research
- Surveys
- User Research
- Marketing Analytics
- ai-personas
- MCP
- Agent-Native
- GDPR
---
