---
api_specs:
- filename: phonic-agents-api-openapi.yml
  format: yaml
  label: Phonic agents API
  slug: phonic-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-agents-api-openapi.yml
- filename: phonic-apikeys-api-openapi.yml
  format: yaml
  label: Phonic apiKeys API
  slug: phonic-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-apikeys-api-openapi.yml
- filename: phonic-auth-api-openapi.yml
  format: yaml
  label: Phonic auth API
  slug: phonic-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-auth-api-openapi.yml
- filename: phonic-conversationitems-api-openapi.yml
  format: yaml
  label: Phonic conversationItems API
  slug: phonic-conversationitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-conversationitems-api-openapi.yml
- filename: phonic-conversations-api-openapi.yml
  format: yaml
  label: Phonic conversations API
  slug: phonic-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-conversations-api-openapi.yml
- filename: phonic-extractionschemas-api-openapi.yml
  format: yaml
  label: Phonic extractionSchemas API
  slug: phonic-extractionschemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-extractionschemas-api-openapi.yml
- filename: phonic-projects-api-openapi.yml
  format: yaml
  label: Phonic projects API
  slug: phonic-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-projects-api-openapi.yml
- filename: phonic-tools-api-openapi.yml
  format: yaml
  label: Phonic tools API
  slug: phonic-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-tools-api-openapi.yml
- filename: phonic-voices-api-openapi.yml
  format: yaml
  label: Phonic voices API
  slug: phonic-voices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-voices-api-openapi.yml
- filename: phonic-workspace-api-openapi.yml
  format: yaml
  label: Phonic workspace API
  slug: phonic-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/openapi/phonic-workspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: phonic.ai
  spf: true
hosts:
- cert_expires: Oct 14 23:42:31 2026 GMT
  host: api.phonic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phonic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Phonic
provider_slug: phonic
slug: phonic-domain-security
source_filename: phonic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.phonic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:42:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: phonic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phonic/refs/heads/main/security/phonic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Voice AI
- Conversational AI
- Speech
- Voice Agents
- Telephony
- Speech To Speech
---
