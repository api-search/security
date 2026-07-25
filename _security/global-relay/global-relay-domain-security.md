---
api_specs:
- filename: global-relay-conversations-api-openapi.yml
  format: yaml
  label: Global Relay Conversations API
  slug: global-relay-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-conversations-api-openapi.yml
- filename: global-relay-email-api-openapi.yml
  format: yaml
  label: Global Relay Email API
  slug: global-relay-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-email-api-openapi.yml
- filename: global-relay-events-api-openapi.yml
  format: yaml
  label: Global Relay Events API
  slug: global-relay-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-events-api-openapi.yml
- filename: global-relay-files-api-openapi.yml
  format: yaml
  label: Global Relay Files API
  slug: global-relay-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-files-api-openapi.yml
- filename: global-relay-voice-api-openapi.yml
  format: yaml
  label: Global Relay Voice API
  slug: global-relay-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/openapi/global-relay-voice-api-openapi.yml
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
