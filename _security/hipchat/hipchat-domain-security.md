---
api_specs:
- filename: hipchat-rest-api-openapi.yml
  format: yaml
  label: HipChat REST API v2
  slug: hipchat-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipchat/refs/heads/main/openapi/hipchat-rest-api-openapi.yml
- filename: hipchat-webhooks-asyncapi.yml
  format: yaml
  label: HipChat Webhooks API
  slug: hipchat-webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/hipchat/refs/heads/main/asyncapi/hipchat-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: atlassian.com
  spf: true
hosts:
- cert_expires: Jan  1 23:59:59 2027 GMT
  host: developer.atlassian.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hipchat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HipChat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HipChat
provider_slug: hipchat
slug: hipchat-domain-security
source_filename: hipchat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.atlassian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: atlassian.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hipchat/refs/heads/main/security/hipchat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Chat
- Messaging
- Collaboration
- Team Communication
- Sunset
- Historical
- Atlassian
- Webhooks
---
