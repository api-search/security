---
api_specs:
- filename: nextiva-authentication-api-openapi.yml
  format: yaml
  label: Nextiva Authentication API
  slug: nextiva-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-authentication-api-openapi.yml
- filename: nextiva-call-management-api-openapi.yml
  format: yaml
  label: Nextiva Call Management API
  slug: nextiva-call-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-call-management-api-openapi.yml
- filename: nextiva-campaigns-api-openapi.yml
  format: yaml
  label: Nextiva Campaigns API
  slug: nextiva-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-campaigns-api-openapi.yml
- filename: nextiva-conversations-api-openapi.yml
  format: yaml
  label: Nextiva Conversations API
  slug: nextiva-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-conversations-api-openapi.yml
- filename: nextiva-dtmf-api-openapi.yml
  format: yaml
  label: Nextiva DTMF API
  slug: nextiva-dtmf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-dtmf-api-openapi.yml
- filename: nextiva-email-api-openapi.yml
  format: yaml
  label: Nextiva Email API
  slug: nextiva-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-email-api-openapi.yml
- filename: nextiva-sms-messaging-api-openapi.yml
  format: yaml
  label: Nextiva SMS Messaging API
  slug: nextiva-sms-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-sms-messaging-api-openapi.yml
- filename: nextiva-tickets-api-openapi.yml
  format: yaml
  label: Nextiva Tickets API
  slug: nextiva-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-tickets-api-openapi.yml
- filename: nextiva-transfers-api-openapi.yml
  format: yaml
  label: Nextiva Transfers API
  slug: nextiva-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-transfers-api-openapi.yml
- filename: nextiva-workitems-api-openapi.yml
  format: yaml
  label: Nextiva Workitems API
  slug: nextiva-workitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/openapi/nextiva-workitems-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nextiva.com
  spf: true
hosts:
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: www.nextiva.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 01:19:27 2026 GMT
  host: developer.nextiva.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 14 23:59:59 2027 GMT
  host: api.nextiva.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nextiva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nextiva, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nextiva
provider_slug: nextiva
slug: nextiva-domain-security
source_filename: nextiva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nextiva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.nextiva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 01:19:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nextiva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nextiva.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextiva/refs/heads/main/security/nextiva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Communications
- Voice
- Contact Center
- Customer Experience
- SMS
- Messaging
- Unified Communications
- VoIP
- Telephony
- Conversational AI
- Call Center
---
