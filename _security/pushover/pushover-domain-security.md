---
api_specs:
- filename: pushover-asyncapi.yml
  format: yaml
  label: Pushover Open Client API
  slug: open-client-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushover/refs/heads/main/openapi/pushover-asyncapi.yml
- filename: pushover-apps-api-openapi.yml
  format: yaml
  label: Pushover Apps API
  slug: pushover-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushover/refs/heads/main/openapi/pushover-apps-api-openapi.yml
- filename: pushover-messages-json-api-openapi.yml
  format: yaml
  label: Pushover Messages.json API
  slug: pushover-messages-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushover/refs/heads/main/openapi/pushover-messages-json-api-openapi.yml
- filename: pushover-receipts-api-openapi.yml
  format: yaml
  label: Pushover Receipts API
  slug: pushover-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushover/refs/heads/main/openapi/pushover-receipts-api-openapi.yml
- filename: pushover-sounds-json-api-openapi.yml
  format: yaml
  label: Pushover Sounds.json API
  slug: pushover-sounds-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushover/refs/heads/main/openapi/pushover-sounds-json-api-openapi.yml
- filename: pushover-users-api-openapi.yml
  format: yaml
  label: Pushover Users API
  slug: pushover-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushover/refs/heads/main/openapi/pushover-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pushover.net
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: pushover.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: api.pushover.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: client.pushover.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pushover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pushover, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pushover
provider_slug: pushover
slug: pushover-domain-security
source_filename: pushover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pushover.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pushover.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: client.pushover.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pushover.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pushover/refs/heads/main/security/pushover-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notification
- Push Notifications
- Messaging
- Alerts
- Monitoring
---
