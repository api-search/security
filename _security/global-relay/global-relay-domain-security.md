---
api_specs:
- filename: global-relay-conversation-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Conversation Archiving API
  slug: conversation-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-conversation-archiving-api-openapi.yml
- filename: global-relay-email-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Email Archiving API
  slug: email-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-email-archiving-api-openapi.yml
- filename: global-relay-voice-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Voice Archiving API
  slug: voice-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-voice-archiving-api-openapi.yml
- filename: global-relay-event-archiving-api-openapi.yml
  format: yaml
  label: Global Relay Event Archiving API
  slug: event-archiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-event-archiving-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: globalrelay.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: developers.globalrelay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: conversations.api.globalrelay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: email.api.globalrelay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Global Relay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Global Relay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Global Relay
provider_slug: global-relay
slug: global-relay-domain-security
source_filename: global-relay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.globalrelay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\n- host: conversations.api.globalrelay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\n- host: email.api.globalrelay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: globalrelay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/security/global-relay-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Archiving
- Compliance
- Data Retention
- Email Security
- Regulatory Compliance
---
