---
api_specs:
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Messaging API
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Conversations API
  slug: conversations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Campaigns API
  slug: campaigns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Sequences API
  slug: sequences
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Channels API
  slug: channels
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
- filename: whippy-openapi.yml
  format: yaml
  label: Whippy Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/openapi/whippy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: whippy.ai
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: whippy.co
  spf: true
hosts:
- cert_expires: Aug 13 23:45:45 2026 GMT
  host: www.whippy.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 20:47:14 2026 GMT
  host: docs.whippy.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 02:40:02 2026 GMT
  host: api.whippy.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whippy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whippy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Whippy
provider_slug: whippy
slug: whippy-domain-security
source_filename: whippy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.whippy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.whippy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 20:47:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.whippy.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 02:40:02 2026 GMT\n  hsts: null\ndomains:\n- domain: whippy.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: whippy.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whippy/refs/heads/main/security/whippy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communication
- Messaging
- SMS
- Email
- Voice
- AI
- Campaigns
- Sequences
---
