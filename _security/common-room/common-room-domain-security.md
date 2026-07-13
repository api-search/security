---
api_specs:
- filename: community.html
  format: yaml
  label: Common Room Core API
  slug: common-room-core-api
  spec_type: OpenAPI
  url: https://api.commonroom.io/docs/community.html
- filename: common-room-scim-openapi.yml
  format: yaml
  label: Common Room SCIM API
  slug: common-room-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/common-room/refs/heads/main/openapi/common-room-scim-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: commonroom.io
  spf: true
hosts:
- cert_expires: Aug 27 19:14:04 2026 GMT
  host: www.commonroom.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: api.commonroom.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Common Room Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Common Room, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Common Room
provider_slug: common-room
slug: common-room-domain-security
source_filename: common-room-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.commonroom.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:14:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.commonroom.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: commonroom.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/common-room/refs/heads/main/security/common-room-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Community Intelligence
- Go-to-Market
- Member Signals
- GitHub
- Slack
- Discord
- LinkedIn
- Sales Intelligence
- Contact Management
- Webhooks
---
