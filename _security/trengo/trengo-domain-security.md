---
api_specs:
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Tickets API
  slug: trengo-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Contacts API
  slug: trengo-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Messages API
  slug: trengo-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Channels API
  slug: trengo-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Teams and Users API
  slug: trengo-teams-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Labels and Custom Fields API
  slug: trengo-labels-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo Webhooks API
  slug: trengo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
- filename: trengo-openapi.yml
  format: yaml
  label: Trengo WhatsApp Templates API
  slug: trengo-whatsapp-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/openapi/trengo-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: trengo.com
  spf: true
hosts:
- cert_expires: Sep 14 08:38:30 2026 GMT
  host: trengo.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 09:58:34 2026 GMT
  host: developers.trengo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 07:26:29 2026 GMT
  host: app.trengo.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trengo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trengo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Trengo
provider_slug: trengo
slug: trengo-domain-security
source_filename: trengo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trengo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:38:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.trengo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:58:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.trengo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 07:26:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: trengo.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trengo/refs/heads/main/security/trengo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Customer Engagement
- Omnichannel
- Shared Inbox
- Messaging
- WhatsApp
- Customer Support
---
