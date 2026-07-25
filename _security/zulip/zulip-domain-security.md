---
api_specs:
- filename: zulip-events-asyncapi.yml
  format: yaml
  label: Zulip REST API
  slug: rest-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/asyncapi/zulip-events-asyncapi.yml
- filename: zulip-events-asyncapi.yml
  format: yaml
  label: Zulip Events API
  slug: events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/asyncapi/zulip-events-asyncapi.yml
- filename: zulip-authentication-api-openapi.yml
  format: yaml
  label: Zulip authentication API
  slug: zulip-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-authentication-api-openapi.yml
- filename: zulip-bots-api-openapi.yml
  format: yaml
  label: Zulip bots API
  slug: zulip-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-bots-api-openapi.yml
- filename: zulip-channels-api-openapi.yml
  format: yaml
  label: Zulip channels API
  slug: zulip-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-channels-api-openapi.yml
- filename: zulip-drafts-api-openapi.yml
  format: yaml
  label: Zulip drafts API
  slug: zulip-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-drafts-api-openapi.yml
- filename: zulip-invites-api-openapi.yml
  format: yaml
  label: Zulip invites API
  slug: zulip-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-invites-api-openapi.yml
- filename: zulip-messages-api-openapi.yml
  format: yaml
  label: Zulip messages API
  slug: zulip-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-messages-api-openapi.yml
- filename: zulip-mobile-api-openapi.yml
  format: yaml
  label: Zulip mobile API
  slug: zulip-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-mobile-api-openapi.yml
- filename: zulip-navigation-views-api-openapi.yml
  format: yaml
  label: Zulip navigation_views API
  slug: zulip-navigation-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-navigation-views-api-openapi.yml
- filename: zulip-real-time-events-api-openapi.yml
  format: yaml
  label: Zulip real_time_events API
  slug: zulip-real-time-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-real-time-events-api-openapi.yml
- filename: zulip-reminders-api-openapi.yml
  format: yaml
  label: Zulip reminders API
  slug: zulip-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-reminders-api-openapi.yml
- filename: zulip-scheduled-messages-api-openapi.yml
  format: yaml
  label: Zulip scheduled_messages API
  slug: zulip-scheduled-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-scheduled-messages-api-openapi.yml
- filename: zulip-server-and-organizations-api-openapi.yml
  format: yaml
  label: Zulip server_and_organizations API
  slug: zulip-server-and-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-server-and-organizations-api-openapi.yml
- filename: zulip-users-api-openapi.yml
  format: yaml
  label: Zulip users API
  slug: zulip-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-users-api-openapi.yml
- filename: zulip-webhooks-api-openapi.yml
  format: yaml
  label: Zulip webhooks API
  slug: zulip-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/openapi/zulip-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zulip.com
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zulip.org
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: zulip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 11:32:09 2026 GMT
  host: chat.zulip.org
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zulip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zulip, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zulip
provider_slug: zulip
slug: zulip-domain-security
source_filename: zulip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zulip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: chat.zulip.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 11:32:09 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: zulip.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zulip.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zulip/refs/heads/main/security/zulip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Messaging
- Team Chat
- Webhooks
---
