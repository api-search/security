---
api_specs:
- filename: telefon-voice-openapi.yml
  format: yaml
  label: Telefon Voice API
  slug: telefon-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-voice-openapi.yml
- filename: telefon-sms-openapi.yml
  format: yaml
  label: Telefon SMS API
  slug: telefon-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-sms-openapi.yml
- filename: telefon-numbers-openapi.yml
  format: yaml
  label: Telefon Number Management API
  slug: telefon-number-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-numbers-openapi.yml
- filename: telefon-recording-openapi.yml
  format: yaml
  label: Telefon Call Recording API
  slug: telefon-call-recording-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefon/refs/heads/main/openapi/telefon-recording-openapi.yml
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
