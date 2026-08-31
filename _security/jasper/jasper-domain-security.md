---
api_specs:
- filename: jasper-attachments-api-openapi.yml
  format: yaml
  label: Jasper Attachments API
  slug: jasper-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-attachments-api-openapi.yml
- filename: jasper-audiences-api-openapi.yml
  format: yaml
  label: Jasper Audiences API
  slug: jasper-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-audiences-api-openapi.yml
- filename: jasper-command-api-openapi.yml
  format: yaml
  label: Jasper Command API
  slug: jasper-command-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-command-api-openapi.yml
- filename: jasper-documents-api-openapi.yml
  format: yaml
  label: Jasper Documents API
  slug: jasper-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-documents-api-openapi.yml
- filename: jasper-image-templates-api-openapi.yml
  format: yaml
  label: Jasper Image Templates API
  slug: jasper-image-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-image-templates-api-openapi.yml
- filename: jasper-images-api-openapi.yml
  format: yaml
  label: Jasper Images API
  slug: jasper-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-images-api-openapi.yml
- filename: jasper-knowledge-api-openapi.yml
  format: yaml
  label: Jasper Knowledge API
  slug: jasper-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-knowledge-api-openapi.yml
- filename: jasper-projects-api-openapi.yml
  format: yaml
  label: Jasper Projects API
  slug: jasper-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-projects-api-openapi.yml
- filename: jasper-styles-api-openapi.yml
  format: yaml
  label: Jasper Styles API
  slug: jasper-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-styles-api-openapi.yml
- filename: jasper-tasks-api-openapi.yml
  format: yaml
  label: Jasper Tasks API
  slug: jasper-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-tasks-api-openapi.yml
- filename: jasper-templates-api-openapi.yml
  format: yaml
  label: Jasper Templates API
  slug: jasper-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-templates-api-openapi.yml
- filename: jasper-usage-api-openapi.yml
  format: yaml
  label: Jasper Usage API
  slug: jasper-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-usage-api-openapi.yml
- filename: jasper-users-api-openapi.yml
  format: yaml
  label: Jasper Users API
  slug: jasper-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-users-api-openapi.yml
- filename: jasper-voices-api-openapi.yml
  format: yaml
  label: Jasper Voices API
  slug: jasper-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-voices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jasper.ai
  spf: true
hosts:
- cert_expires: Nov 11 09:20:57 2026 GMT
  host: www.jasper.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 15:55:51 2026 GMT
  host: developers.jasper.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 13:49:10 2026 GMT
  host: api.jasper.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jasper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jasper, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jasper
provider_slug: jasper
slug: jasper-domain-security
source_filename: jasper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jasper.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 09:20:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.jasper.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:55:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.jasper.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 13:49:10 2026 GMT\n  hsts: null\ndomains:\n- domain: jasper.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/security/jasper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Content Generation
- Marketing
- Generative AI
- Agents
- MCP
---
