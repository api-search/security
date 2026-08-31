---
api_specs:
- filename: novu-asyncapi.yml
  format: yaml
  label: Novu Inbox / In-App API
  slug: inbox-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/asyncapi/novu-asyncapi.yml
- filename: novu-activity-api-openapi.yml
  format: yaml
  label: Novu Activity API
  slug: novu-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-activity-api-openapi.yml
- filename: novu-channel-connections-api-openapi.yml
  format: yaml
  label: Novu Channel Connections API
  slug: novu-channel-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-channel-connections-api-openapi.yml
- filename: novu-channel-endpoints-api-openapi.yml
  format: yaml
  label: Novu Channel Endpoints API
  slug: novu-channel-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-channel-endpoints-api-openapi.yml
- filename: novu-contexts-api-openapi.yml
  format: yaml
  label: Novu Contexts API
  slug: novu-contexts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-contexts-api-openapi.yml
- filename: novu-domains-api-openapi.yml
  format: yaml
  label: Novu Domains API
  slug: novu-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-domains-api-openapi.yml
- filename: novu-environment-variables-api-openapi.yml
  format: yaml
  label: Novu Environment Variables API
  slug: novu-environment-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-environment-variables-api-openapi.yml
- filename: novu-environments-api-openapi.yml
  format: yaml
  label: Novu Environments API
  slug: novu-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-environments-api-openapi.yml
- filename: novu-events-api-openapi.yml
  format: yaml
  label: Novu Events API
  slug: novu-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-events-api-openapi.yml
- filename: novu-integrations-api-openapi.yml
  format: yaml
  label: Novu Integrations API
  slug: novu-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-integrations-api-openapi.yml
- filename: novu-layouts-api-openapi.yml
  format: yaml
  label: Novu Layouts API
  slug: novu-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-layouts-api-openapi.yml
- filename: novu-messages-api-openapi.yml
  format: yaml
  label: Novu Messages API
  slug: novu-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-messages-api-openapi.yml
- filename: novu-notifications-api-openapi.yml
  format: yaml
  label: Novu Notifications API
  slug: novu-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-notifications-api-openapi.yml
- filename: novu-subscribers-api-openapi.yml
  format: yaml
  label: Novu Subscribers API
  slug: novu-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-subscribers-api-openapi.yml
- filename: novu-topics-api-openapi.yml
  format: yaml
  label: Novu Topics API
  slug: novu-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-topics-api-openapi.yml
- filename: novu-translations-api-openapi.yml
  format: yaml
  label: Novu Translations API
  slug: novu-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-translations-api-openapi.yml
- filename: novu-workflows-api-openapi.yml
  format: yaml
  label: Novu Workflows API
  slug: novu-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-workflows-api-openapi.yml
- filename: novu-webhooks-api-openapi.yml
  format: yaml
  label: Novu Webhooks API
  slug: novu-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/openapi/novu-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: novu.co
  spf: true
hosts:
- cert_expires: Oct  7 13:09:55 2026 GMT
  host: novu.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 05:09:47 2026 GMT
  host: docs.novu.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 21:15:28 2026 GMT
  host: api.novu.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Novu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Novu, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Novu
provider_slug: novu
slug: novu-domain-security
source_filename: novu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 13:09:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.novu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:09:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.novu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 21:15:28 2026 GMT\n  hsts: null\ndomains:\n- domain: novu.co\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novu/refs/heads/main/security/novu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notification
- Messaging
- In App
- Email
- SMS
- Push
- Chat
- Workflows
- Open-Source
- Subscribers
- Topics
- Inbox
- Workflow Orchestration
- Multi Channel
- Digest
- MCP
- Framework
- React
---
