---
api_specs:
- filename: flowise-assistants-api-openapi.yml
  format: yaml
  label: Flowise assistants API
  slug: flowise-assistants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-assistants-api-openapi.yml
- filename: flowise-attachments-api-openapi.yml
  format: yaml
  label: Flowise attachments API
  slug: flowise-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-attachments-api-openapi.yml
- filename: flowise-chatflows-api-openapi.yml
  format: yaml
  label: Flowise chatflows API
  slug: flowise-chatflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-chatflows-api-openapi.yml
- filename: flowise-chatmessage-api-openapi.yml
  format: yaml
  label: Flowise chatmessage API
  slug: flowise-chatmessage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-chatmessage-api-openapi.yml
- filename: flowise-document-store-api-openapi.yml
  format: yaml
  label: Flowise document-store API
  slug: flowise-document-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-document-store-api-openapi.yml
- filename: flowise-feedback-api-openapi.yml
  format: yaml
  label: Flowise feedback API
  slug: flowise-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-feedback-api-openapi.yml
- filename: flowise-leads-api-openapi.yml
  format: yaml
  label: Flowise leads API
  slug: flowise-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-leads-api-openapi.yml
- filename: flowise-ping-api-openapi.yml
  format: yaml
  label: Flowise ping API
  slug: flowise-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-ping-api-openapi.yml
- filename: flowise-prediction-api-openapi.yml
  format: yaml
  label: Flowise prediction API
  slug: flowise-prediction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-prediction-api-openapi.yml
- filename: flowise-tools-api-openapi.yml
  format: yaml
  label: Flowise tools API
  slug: flowise-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-tools-api-openapi.yml
- filename: flowise-upsert-history-api-openapi.yml
  format: yaml
  label: Flowise upsert-history API
  slug: flowise-upsert-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-upsert-history-api-openapi.yml
- filename: flowise-variables-api-openapi.yml
  format: yaml
  label: Flowise variables API
  slug: flowise-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-variables-api-openapi.yml
- filename: flowise-vector-api-openapi.yml
  format: yaml
  label: Flowise vector API
  slug: flowise-vector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/openapi/flowise-vector-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flowiseai.com
  spf: true
hosts:
- cert_expires: Aug 21 09:49:24 2026 GMT
  host: flowiseai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 03:02:32 2026 GMT
  host: docs.flowiseai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flowise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flowise, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flowise
provider_slug: flowise
slug: flowise-domain-security
source_filename: flowise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowiseai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 09:49:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.flowiseai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:02:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: flowiseai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowise/refs/heads/main/security/flowise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Agent Workflows
- Artificial Intelligence
- Large Language Models
- Low-Code
- Visual Builder
- LangChain
- RAG
- Retrieval Augmented Generation
- Chatbots
- Open-Source
- Node.js
- TypeScript
---
