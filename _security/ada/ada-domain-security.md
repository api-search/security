---
api_specs:
- filename: ada-subpackage-channels-api-openapi.yml
  format: yaml
  label: Ada subpackage_channels API
  slug: ada-subpackage-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-channels-api-openapi.yml
- filename: ada-subpackage-conversations-api-openapi.yml
  format: yaml
  label: Ada subpackage_conversations API
  slug: ada-subpackage-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-conversations-api-openapi.yml
- filename: ada-subpackage-deletechatterdata-api-openapi.yml
  format: yaml
  label: Ada subpackage_deleteChatterData API
  slug: ada-subpackage-deletechatterdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-deletechatterdata-api-openapi.yml
- filename: ada-subpackage-endusers-api-openapi.yml
  format: yaml
  label: Ada subpackage_endUsers API
  slug: ada-subpackage-endusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-endusers-api-openapi.yml
- filename: ada-subpackage-knowledge-subpackage-knowledge-articles-api-openapi.yml
  format: yaml
  label: Ada subpackage_knowledge.subpackage_knowledge/articles API
  slug: ada-subpackage-knowledge-subpackage-knowledge-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-knowledge-subpackage-knowledge-articles-api-openapi.yml
- filename: ada-subpackage-knowledge-subpackage-knowledge-sources-api-openapi.yml
  format: yaml
  label: Ada subpackage_knowledge.subpackage_knowledge/sources API
  slug: ada-subpackage-knowledge-subpackage-knowledge-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-knowledge-subpackage-knowledge-sources-api-openapi.yml
- filename: ada-subpackage-knowledge-subpackage-knowledge-tags-api-openapi.yml
  format: yaml
  label: Ada subpackage_knowledge.subpackage_knowledge/tags API
  slug: ada-subpackage-knowledge-subpackage-knowledge-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-knowledge-subpackage-knowledge-tags-api-openapi.yml
- filename: ada-subpackage-messages-api-openapi.yml
  format: yaml
  label: Ada subpackage_messages API
  slug: ada-subpackage-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-messages-api-openapi.yml
- filename: ada-subpackage-platformintegrations-api-openapi.yml
  format: yaml
  label: Ada subpackage_platformIntegrations API
  slug: ada-subpackage-platformintegrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-platformintegrations-api-openapi.yml
- filename: ada-subpackage-webhookmanagement-api-openapi.yml
  format: yaml
  label: Ada subpackage_webhookManagement API
  slug: ada-subpackage-webhookmanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-webhookmanagement-api-openapi.yml
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
