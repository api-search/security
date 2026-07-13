---
api_specs:
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Events API
  slug: novu-co-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Subscribers API
  slug: novu-co-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Topics API
  slug: novu-co-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Inbox API
  slug: novu-co-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Messages API
  slug: novu-co-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Notifications API
  slug: novu-co-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Workflows API
  slug: novu-co-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Integrations API
  slug: novu-co-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Layouts API
  slug: novu-co-layouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Subscriber Preferences API
  slug: novu-co-subscriber-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Environments API
  slug: novu-co-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-openapi.yml
  format: yaml
  label: Novu Translations API
  slug: novu-co-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/openapi/novu-co-openapi.yml
- filename: novu-co-asyncapi.yml
  format: yaml
  label: Novu Inbox Realtime API
  slug: novu-co-inbox-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/asyncapi/novu-co-asyncapi.yml
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
name: Novu Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Novu, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Novu
provider_slug: novu-co
slug: novu-co-domain-security
source_filename: novu-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 13:09:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.novu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:09:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.novu.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 21:15:28 2026 GMT\n  hsts: null\ndomains:\n- domain: novu.co\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novu-co/refs/heads/main/security/novu-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notifications
- Multi-Channel
- Email
- SMS
- Push
- Chat
- In-App Inbox
- Open Source
- WebSocket
---
