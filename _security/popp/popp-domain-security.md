---
api_specs:
- filename: popp-agents-api-openapi.yml
  format: yaml
  label: Popp Agents API
  slug: popp-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-agents-api-openapi.yml
- filename: popp-analysis-api-openapi.yml
  format: yaml
  label: Popp Analysis API
  slug: popp-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-analysis-api-openapi.yml
- filename: popp-ats-api-openapi.yml
  format: yaml
  label: Popp ATS API
  slug: popp-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-ats-api-openapi.yml
- filename: popp-campaigns-api-openapi.yml
  format: yaml
  label: Popp Campaigns API
  slug: popp-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-campaigns-api-openapi.yml
- filename: popp-candidate-lists-api-openapi.yml
  format: yaml
  label: Popp Candidate Lists API
  slug: popp-candidate-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-candidate-lists-api-openapi.yml
- filename: popp-candidates-api-openapi.yml
  format: yaml
  label: Popp Candidates API
  slug: popp-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-candidates-api-openapi.yml
- filename: popp-conversations-api-openapi.yml
  format: yaml
  label: Popp Conversations API
  slug: popp-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-conversations-api-openapi.yml
- filename: popp-custom-fields-beta-api-openapi.yml
  format: yaml
  label: Popp Custom Fields (Beta) API
  slug: popp-custom-fields-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-custom-fields-beta-api-openapi.yml
- filename: popp-document-credentials-api-openapi.yml
  format: yaml
  label: Popp Document Credentials API
  slug: popp-document-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-document-credentials-api-openapi.yml
- filename: popp-documents-api-openapi.yml
  format: yaml
  label: Popp Documents API
  slug: popp-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-documents-api-openapi.yml
- filename: popp-organization-configuration-api-openapi.yml
  format: yaml
  label: Popp Organization Configuration API
  slug: popp-organization-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-organization-configuration-api-openapi.yml
- filename: popp-organizations-api-openapi.yml
  format: yaml
  label: Popp Organizations API
  slug: popp-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-organizations-api-openapi.yml
- filename: popp-scheduling-api-openapi.yml
  format: yaml
  label: Popp Scheduling API
  slug: popp-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-scheduling-api-openapi.yml
- filename: popp-tags-api-openapi.yml
  format: yaml
  label: Popp Tags API
  slug: popp-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-tags-api-openapi.yml
- filename: popp-templates-api-openapi.yml
  format: yaml
  label: Popp Templates API
  slug: popp-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-templates-api-openapi.yml
- filename: popp-users-api-openapi.yml
  format: yaml
  label: Popp Users API
  slug: popp-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-users-api-openapi.yml
- filename: popp-webhooks-api-openapi.yml
  format: yaml
  label: Popp Webhooks API
  slug: popp-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-webhooks-api-openapi.yml
- filename: popp-workflows-api-openapi.yml
  format: yaml
  label: Popp Workflows API
  slug: popp-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/openapi/popp-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joinpopp.com
  spf: true
hosts:
- cert_expires: Oct 15 10:16:54 2026 GMT
  host: joinpopp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Popp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Popp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Popp
provider_slug: popp
slug: popp-domain-security
source_filename: popp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinpopp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 10:16:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: joinpopp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popp/refs/heads/main/security/popp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Staffing
- Hiring
- Conversational AI
- Automation
- Scheduling
- Workflows
- Webhook
- MCP
- Agents
---
