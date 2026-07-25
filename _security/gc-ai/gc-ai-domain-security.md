---
api_specs:
- filename: gc-ai-chat-api-openapi.yml
  format: yaml
  label: GC AI Chat API
  slug: gc-ai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-chat-api-openapi.yml
- filename: gc-ai-files-api-openapi.yml
  format: yaml
  label: GC AI Files API
  slug: gc-ai-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-files-api-openapi.yml
- filename: gc-ai-folders-api-openapi.yml
  format: yaml
  label: GC AI Folders API
  slug: gc-ai-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-folders-api-openapi.yml
- filename: gc-ai-playbooks-api-openapi.yml
  format: yaml
  label: GC AI Playbooks API
  slug: gc-ai-playbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-playbooks-api-openapi.yml
- filename: gc-ai-profiles-api-openapi.yml
  format: yaml
  label: GC AI Profiles API
  slug: gc-ai-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-profiles-api-openapi.yml
- filename: gc-ai-projects-api-openapi.yml
  format: yaml
  label: GC AI Projects API
  slug: gc-ai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-projects-api-openapi.yml
- filename: gc-ai-skills-api-openapi.yml
  format: yaml
  label: GC AI Skills API
  slug: gc-ai-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-skills-api-openapi.yml
- filename: gc-ai-usage-api-openapi.yml
  format: yaml
  label: GC AI Usage API
  slug: gc-ai-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-usage-api-openapi.yml
- filename: gc-ai-utility-api-openapi.yml
  format: yaml
  label: GC AI Utility API
  slug: gc-ai-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/openapi/gc-ai-utility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gc.ai
  spf: true
hosts:
- cert_expires: Sep 18 20:39:10 2026 GMT
  host: gc.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 15:09:26 2026 GMT
  host: app.gc.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gc Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GC AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: GC AI
provider_slug: gc-ai
slug: gc-ai-domain-security
source_filename: gc-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gc.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:39:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.gc.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:09:26 2026 GMT\n  hsts: false\ndomains:\n- domain: gc.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gc-ai/refs/heads/main/security/gc-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Legal
- Legal AI
- Contracts
- In-House Counsel
- Artificial Intelligence
- Document Review
- Enterprise
- MCP
---
