---
api_specs:
- filename: ada-conversations-api-openapi.yml
  format: yaml
  label: Ada Conversations API
  slug: ada-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-conversations-api-openapi.yml
- filename: ada-auditlog-api-openapi.yml
  format: yaml
  label: Ada Audit Log API
  slug: ada-auditlog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-auditlog-api-openapi.yml
- filename: ada-channels-api-openapi.yml
  format: yaml
  label: Ada Channels API
  slug: ada-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-channels-api-openapi.yml
- filename: ada-conversations-api-openapi.yml
  format: yaml
  label: Ada Conversations API
  slug: ada-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-conversations-api-openapi.yml
- filename: ada-custominstructions-api-openapi.yml
  format: yaml
  label: Ada Custom Instructions API
  slug: ada-custominstructions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-custominstructions-api-openapi.yml
- filename: ada-deletechatterdata-api-openapi.yml
  format: yaml
  label: Ada Delete Chatter Data API
  slug: ada-deletechatterdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-deletechatterdata-api-openapi.yml
- filename: ada-endusers-api-openapi.yml
  format: yaml
  label: Ada End Users API
  slug: ada-endusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-endusers-api-openapi.yml
- filename: ada-getdeletionjob-api-openapi.yml
  format: yaml
  label: Ada Get Deletion Job API
  slug: ada-getdeletionjob-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-getdeletionjob-api-openapi.yml
- filename: ada-knowledge-api-openapi.yml
  format: yaml
  label: Ada Knowledge API
  slug: ada-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-knowledge-api-openapi.yml
- filename: ada-knowledge-articles-api-openapi.yml
  format: yaml
  label: Ada knowledge > articles API
  slug: ada-knowledge-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-knowledge-articles-api-openapi.yml
- filename: ada-knowledge-sources-api-openapi.yml
  format: yaml
  label: Ada knowledge > sources API
  slug: ada-knowledge-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-knowledge-sources-api-openapi.yml
- filename: ada-knowledge-tags-api-openapi.yml
  format: yaml
  label: Ada knowledge > tags API
  slug: ada-knowledge-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-knowledge-tags-api-openapi.yml
- filename: ada-messages-api-openapi.yml
  format: yaml
  label: Ada Messages API
  slug: ada-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-messages-api-openapi.yml
- filename: ada-persona-api-openapi.yml
  format: yaml
  label: Ada Persona API
  slug: ada-persona-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-persona-api-openapi.yml
- filename: ada-platformintegrations-api-openapi.yml
  format: yaml
  label: Ada Platform Integrations API
  slug: ada-platformintegrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-platformintegrations-api-openapi.yml
- filename: ada-submitdeletionrequest-api-openapi.yml
  format: yaml
  label: Ada Submit Deletion Request API
  slug: ada-submitdeletionrequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-submitdeletionrequest-api-openapi.yml
- filename: ada-variables-api-openapi.yml
  format: yaml
  label: Ada Variables API
  slug: ada-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-variables-api-openapi.yml
- filename: ada-webhookmanagement-api-openapi.yml
  format: yaml
  label: Ada Webhook Management API
  slug: ada-webhookmanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-webhookmanagement-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonzonaws.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ada.cx
  spf: true
hosts:
- cert_expires: Oct 19 23:39:47 2026 GMT
  host: www.ada.cx
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 06:00:37 2026 GMT
  host: docs.ada.cx
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.ada.cx
  https: false
kind: domain-security
layout: security
method: probed
name: Ada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ada, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ada
provider_slug: ada
slug: ada-domain-security
source_filename: ada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ada.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:39:47 2026 GMT\n  hsts: null\n- host: docs.ada.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 06:00:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ada.cx\n  https: false\ndomains:\n- domain: ada.cx\n  dnssec: true\n  caa:\n  - 0 issue \"amazonzonaws.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/security/ada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Customer Service
- Chatbots
- Automation
- Conversational AI
- Help Desk
- CRM
- Integration
- Knowledge-Management
- Data Export
---
