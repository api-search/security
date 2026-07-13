---
api_specs:
- filename: telefoon-voice-openapi.yml
  format: yaml
  label: Telefoon Voice API
  slug: telefoon-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/openapi/telefoon-voice-openapi.yml
- filename: telefoon-sms-openapi.yml
  format: yaml
  label: Telefoon SMS API
  slug: telefoon-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/openapi/telefoon-sms-openapi.yml
- filename: telefoon-numbers-openapi.yml
  format: yaml
  label: Telefoon Number Management API
  slug: telefoon-number-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/openapi/telefoon-numbers-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: telefoon.com
  spf: false
hosts:
- host: developers.telefoon.com
  https: false
- host: api.telefoon.com
  https: false
kind: domain-security
layout: security
method: probed
name: Telefoon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telefoon, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Telefoon
provider_slug: telefoon
slug: telefoon-domain-security
source_filename: telefoon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.telefoon.com\n  https: false\n- host: api.telefoon.com\n  https: false\ndomains:\n- domain: telefoon.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telefoon/refs/heads/main/security/telefoon-domain-security.yml
summary_line: DNSSEC
tags:
- Belgium
- CPaaS
- EU Data Residency
- Europe
- GDPR Compliant
- Messaging
- Netherlands
- Number Provisioning
- SMS
- Telephony
- Voice
---
