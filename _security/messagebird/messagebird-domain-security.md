---
api_specs:
- filename: messagebird-bird-api-openapi.yml
  format: yaml
  label: Bird API
  slug: bird-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-bird-api-openapi.yml
- filename: messagebird-available-numbers-api-openapi.yml
  format: yaml
  label: messagebird Available Numbers API
  slug: messagebird-available-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-available-numbers-api-openapi.yml
- filename: messagebird-balance-api-openapi.yml
  format: yaml
  label: messagebird Balance API
  slug: messagebird-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-balance-api-openapi.yml
- filename: messagebird-call-flows-api-openapi.yml
  format: yaml
  label: messagebird Call Flows API
  slug: messagebird-call-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-call-flows-api-openapi.yml
- filename: messagebird-calls-api-openapi.yml
  format: yaml
  label: messagebird Calls API
  slug: messagebird-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-calls-api-openapi.yml
- filename: messagebird-contacts-api-openapi.yml
  format: yaml
  label: messagebird Contacts API
  slug: messagebird-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-contacts-api-openapi.yml
- filename: messagebird-conversations-api-openapi.yml
  format: yaml
  label: messagebird Conversations API
  slug: messagebird-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-conversations-api-openapi.yml
- filename: messagebird-groups-api-openapi.yml
  format: yaml
  label: messagebird Groups API
  slug: messagebird-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-groups-api-openapi.yml
- filename: messagebird-hlr-api-openapi.yml
  format: yaml
  label: messagebird HLR API
  slug: messagebird-hlr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-hlr-api-openapi.yml
- filename: messagebird-legs-api-openapi.yml
  format: yaml
  label: messagebird Legs API
  slug: messagebird-legs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-legs-api-openapi.yml
- filename: messagebird-lookup-api-openapi.yml
  format: yaml
  label: messagebird Lookup API
  slug: messagebird-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-lookup-api-openapi.yml
- filename: messagebird-messages-api-openapi.yml
  format: yaml
  label: messagebird Messages API
  slug: messagebird-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-messages-api-openapi.yml
- filename: messagebird-purchased-numbers-api-openapi.yml
  format: yaml
  label: messagebird Purchased Numbers API
  slug: messagebird-purchased-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-purchased-numbers-api-openapi.yml
- filename: messagebird-recordings-api-openapi.yml
  format: yaml
  label: messagebird Recordings API
  slug: messagebird-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-recordings-api-openapi.yml
- filename: messagebird-templates-api-openapi.yml
  format: yaml
  label: messagebird Templates API
  slug: messagebird-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-templates-api-openapi.yml
- filename: messagebird-transcriptions-api-openapi.yml
  format: yaml
  label: messagebird Transcriptions API
  slug: messagebird-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-transcriptions-api-openapi.yml
- filename: messagebird-verify-api-openapi.yml
  format: yaml
  label: messagebird Verify API
  slug: messagebird-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-verify-api-openapi.yml
- filename: messagebird-voice-messages-api-openapi.yml
  format: yaml
  label: messagebird Voice Messages API
  slug: messagebird-voice-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-voice-messages-api-openapi.yml
- filename: messagebird-webhooks-api-openapi.yml
  format: yaml
  label: messagebird Webhooks API
  slug: messagebird-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/openapi/messagebird-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "trust-provider.com"
  - 0 issue "usertrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: messagebird.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: messagebird.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 21:11:04 2026 GMT
  host: developers.messagebird.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 03:55:57 2026 GMT
  host: rest.messagebird.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Messagebird Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Messagebird, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Messagebird
provider_slug: messagebird
slug: messagebird-domain-security
source_filename: messagebird-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: messagebird.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.messagebird.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 21:11:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest.messagebird.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 03:55:57 2026 GMT\n  hsts: null\ndomains:\n- domain: messagebird.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"trust-provider.com\"\n  - 0 issue \"usertrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/messagebird/refs/heads/main/security/messagebird-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications
- Messaging
- SMS
- Email
- WhatsApp
- Voice
- Verification
- CPaaS
- Webhook
- Agents
---
