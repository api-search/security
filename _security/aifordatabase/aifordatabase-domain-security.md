---
api_specs:
- filename: aifordatabase-chat-api-openapi.yml
  format: yaml
  label: AI for Database Chat API
  slug: aifordatabase-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-chat-api-openapi.yml
- filename: aifordatabase-connections-api-openapi.yml
  format: yaml
  label: AI for Database Connections API
  slug: aifordatabase-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-connections-api-openapi.yml
- filename: aifordatabase-conversations-api-openapi.yml
  format: yaml
  label: AI for Database Conversations API
  slug: aifordatabase-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-conversations-api-openapi.yml
- filename: aifordatabase-dashboards-api-openapi.yml
  format: yaml
  label: AI for Database Dashboards API
  slug: aifordatabase-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-dashboards-api-openapi.yml
- filename: aifordatabase-keys-api-openapi.yml
  format: yaml
  label: AI for Database Keys API
  slug: aifordatabase-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-keys-api-openapi.yml
- filename: aifordatabase-metrics-api-openapi.yml
  format: yaml
  label: AI for Database Metrics API
  slug: aifordatabase-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-metrics-api-openapi.yml
- filename: aifordatabase-query-approval-api-openapi.yml
  format: yaml
  label: AI for Database Query Approval API
  slug: aifordatabase-query-approval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-query-approval-api-openapi.yml
- filename: aifordatabase-saved-queries-api-openapi.yml
  format: yaml
  label: AI for Database Saved Queries API
  slug: aifordatabase-saved-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-saved-queries-api-openapi.yml
- filename: aifordatabase-usage-api-openapi.yml
  format: yaml
  label: AI for Database Usage API
  slug: aifordatabase-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-usage-api-openapi.yml
- filename: aifordatabase-webhooks-api-openapi.yml
  format: yaml
  label: AI for Database Webhooks API
  slug: aifordatabase-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-webhooks-api-openapi.yml
- filename: aifordatabase-workflow-credentials-api-openapi.yml
  format: yaml
  label: AI for Database Workflow Credentials API
  slug: aifordatabase-workflow-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-workflow-credentials-api-openapi.yml
- filename: aifordatabase-workflows-api-openapi.yml
  format: yaml
  label: AI for Database Workflows API
  slug: aifordatabase-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/openapi/aifordatabase-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aifordatabase.com
  spf: true
hosts:
- cert_expires: Oct 10 01:52:18 2026 GMT
  host: aifordatabase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 02:44:30 2026 GMT
  host: app.aifordatabase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aifordatabase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI for Database, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AI for Database
provider_slug: aifordatabase
slug: aifordatabase-domain-security
source_filename: aifordatabase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aifordatabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 01:52:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.aifordatabase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 02:44:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aifordatabase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aifordatabase/refs/heads/main/security/aifordatabase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Database
- Analytics
- Developer Tools
- Natural Language Query
- Text-to-SQL
- Dashboards
- Business Intelligence
- Workflow-Automation
- Alerts
- agent-native
- llms-txt
- OpenAPI
- Webhook
- MCP
- PostgreSQL
- MySQL
- MongoDB
---
