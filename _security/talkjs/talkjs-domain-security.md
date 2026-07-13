---
api_specs:
- filename: talkjs-openapi.yml
  format: yaml
  label: TalkJS Users API
  slug: talkjs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkjs/refs/heads/main/openapi/talkjs-openapi.yml
- filename: talkjs-openapi.yml
  format: yaml
  label: TalkJS Conversations & Participants API
  slug: talkjs-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkjs/refs/heads/main/openapi/talkjs-openapi.yml
- filename: talkjs-openapi.yml
  format: yaml
  label: TalkJS Messages API
  slug: talkjs-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkjs/refs/heads/main/openapi/talkjs-openapi.yml
- filename: talkjs-openapi.yml
  format: yaml
  label: TalkJS Import API
  slug: talkjs-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/talkjs/refs/heads/main/openapi/talkjs-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: talkjs.com
  spf: true
hosts:
- cert_expires: Sep  5 16:49:02 2026 GMT
  host: talkjs.com
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talkjs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TalkJS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: TalkJS
provider_slug: talkjs
slug: talkjs-domain-security
source_filename: talkjs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talkjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 16:49:02 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\ndomains:\n- domain: talkjs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkjs/refs/heads/main/security/talkjs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Chat
- Messaging
- Communication
- SDK
- Webhooks
---
