---
api_specs:
- filename: knock-workflows-api-openapi.yml
  format: yaml
  label: Knock Workflows API
  slug: knock-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-workflows-api-openapi.yml
- filename: knock-users-api-openapi.yml
  format: yaml
  label: Knock Users API
  slug: knock-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-users-api-openapi.yml
- filename: knock-messages-api-openapi.yml
  format: yaml
  label: Knock Messages API
  slug: knock-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-messages-api-openapi.yml
- filename: knock-objects-api-openapi.yml
  format: yaml
  label: Knock Objects API
  slug: knock-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-objects-api-openapi.yml
- filename: knock-tenants-api-openapi.yml
  format: yaml
  label: Knock Tenants API
  slug: knock-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-tenants-api-openapi.yml
- filename: knock-schedules-api-openapi.yml
  format: yaml
  label: Knock Schedules API
  slug: knock-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-schedules-api-openapi.yml
- filename: knock-audiences-api-openapi.yml
  format: yaml
  label: Knock Audiences API
  slug: knock-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-audiences-api-openapi.yml
- filename: knock-channels-api-openapi.yml
  format: yaml
  label: Knock Channels API
  slug: knock-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-channels-api-openapi.yml
- filename: knock-providers-api-openapi.yml
  format: yaml
  label: Knock Providers API
  slug: knock-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-providers-api-openapi.yml
- filename: knock-integrations-api-openapi.yml
  format: yaml
  label: Knock Integrations API
  slug: knock-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-integrations-api-openapi.yml
- filename: knock-bulk-operations-api-openapi.yml
  format: yaml
  label: Knock Bulk Operations API
  slug: knock-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-bulk-operations-api-openapi.yml
- filename: knock-notify-api-openapi.yml
  format: yaml
  label: Knock Notify API
  slug: knock-notify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-notify-api-openapi.yml
- filename: knock-management-api-openapi.yml
  format: yaml
  label: Knock Management API (mAPI)
  slug: knock-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/openapi/knock-management-api-openapi.yml
- filename: knock-webhooks-asyncapi.yml
  format: yaml
  label: Knock Outbound Webhooks
  slug: knock-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/asyncapi/knock-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: knock.app
  spf: true
hosts:
- cert_expires: Sep 20 15:29:52 2026 GMT
  host: knock.app
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 21:07:44 2026 GMT
  host: docs.knock.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.knock.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knock App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knock, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Knock
provider_slug: knock-app
slug: knock-app-domain-security
source_filename: knock-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knock.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:29:52 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.knock.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:07:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.knock.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: knock.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knock-app/refs/heads/main/security/knock-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notifications
- Messaging
- Infrastructure
- Workflows
- Cross-Channel
- Email
- SMS
- Push
- In-App
- Chat
- Slack
- Webhooks
- MCP
- AI Agents
- Developer Platform
---
