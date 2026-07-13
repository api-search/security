---
api_specs:
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks SMS API
  slug: 46elks-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks MMS API
  slug: 46elks-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Voice Calls API
  slug: 46elks-voice-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Phone Numbers API
  slug: 46elks-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Media API
  slug: 46elks-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
- filename: 46elks-openapi.yml
  format: yaml
  label: 46elks Verification API
  slug: 46elks-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/openapi/46elks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 46elks.com
  spf: true
hosts:
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: 46elks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: api.46elks.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: 46Elks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 46elks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 46elks
provider_slug: 46elks
slug: 46elks-domain-security
source_filename: 46elks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 46elks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.46elks.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 46elks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/46elks/refs/heads/main/security/46elks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CPaaS
- SMS
- MMS
- Voice
- Messaging
- Phone Numbers
- Communications
---
