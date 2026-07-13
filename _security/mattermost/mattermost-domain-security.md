---
api_specs:
- filename: mattermost-openapi.yml
  format: yaml
  label: Mattermost REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermost/refs/heads/main/openapi/mattermost-openapi.yml
- filename: mattermost-asyncapi.yml
  format: yaml
  label: Mattermost WebSocket API
  slug: websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermost/refs/heads/main/asyncapi/mattermost-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mattermost.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-mattermost-server.com
  spf: false
hosts:
- cert_expires: Sep 14 05:13:33 2026 GMT
  host: mattermost.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.mattermost.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your-mattermost-server.com
  https: false
kind: domain-security
layout: security
method: probed
name: Mattermost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mattermost, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mattermost
provider_slug: mattermost
slug: mattermost-domain-security
source_filename: mattermost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mattermost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:13:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mattermost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-mattermost-server.com\n  https: false\ndomains:\n- domain: mattermost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: your-mattermost-server.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mattermost/refs/heads/main/security/mattermost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Collaboration
- Team Chat
- Open Source
- DevOps
- Self-Hosted
---
