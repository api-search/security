---
api_specs:
- filename: telefon-available-numbers-api-openapi.yml
  format: yaml
  label: Telefon Available Numbers API
  slug: telefon-available-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-available-numbers-api-openapi.yml
- filename: telefon-calls-api-openapi.yml
  format: yaml
  label: Telefon Calls API
  slug: telefon-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-calls-api-openapi.yml
- filename: telefon-conferences-api-openapi.yml
  format: yaml
  label: Telefon Conferences API
  slug: telefon-conferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-conferences-api-openapi.yml
- filename: telefon-messages-api-openapi.yml
  format: yaml
  label: Telefon Messages API
  slug: telefon-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-messages-api-openapi.yml
- filename: telefon-owned-numbers-api-openapi.yml
  format: yaml
  label: Telefon Owned Numbers API
  slug: telefon-owned-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-owned-numbers-api-openapi.yml
- filename: telefon-recordings-api-openapi.yml
  format: yaml
  label: Telefon Recordings API
  slug: telefon-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-recordings-api-openapi.yml
- filename: telefon-transcriptions-api-openapi.yml
  format: yaml
  label: Telefon Transcriptions API
  slug: telefon-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-transcriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: telefon.com
  spf: false
hosts:
- host: developers.telefon.com
  https: false
- host: api.telefon.com
  https: false
kind: domain-security
layout: security
method: probed
name: Telefon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telefon, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Telefon
provider_slug: telefon
slug: telefon-domain-security
source_filename: telefon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.telefon.com\n  https: false\n- host: api.telefon.com\n  https: false\ndomains:\n- domain: telefon.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/security/telefon-domain-security.yml
summary_line: DMARC
tags:
- Call Recording
- Communications
- CPaaS
- Global Coverage
- Messaging
- Number Provisioning
- SMS
- Telephony
- Voice
- VoIP
---
