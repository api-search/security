---
api_specs:
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Send API
  slug: notificationapi-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Schedule API
  slug: notificationapi-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Users Identify API
  slug: notificationapi-users-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI User Preferences API
  slug: notificationapi-user-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Notifications Config API
  slug: notificationapi-notifications-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI In-App Inbox API
  slug: notificationapi-in-app-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
- filename: notificationapi-openapi.yml
  format: yaml
  label: NotificationAPI Logs API
  slug: notificationapi-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/openapi/notificationapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: notificationapi.com
  spf: false
hosts:
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: www.notificationapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: docs.notificationapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Notificationapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NotificationAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: NotificationAPI
provider_slug: notificationapi
slug: notificationapi-domain-security
source_filename: notificationapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.notificationapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.notificationapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: notificationapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notificationapi/refs/heads/main/security/notificationapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notifications
- Messaging
- Email
- SMS
- Push
- In-App Inbox
---
