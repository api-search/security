---
api_specs:
- filename: freshchat-openapi.yml
  format: yaml
  label: Freshchat REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/openapi/freshchat-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freshworks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freshchat.com
  spf: true
hosts:
- cert_expires: Aug 22 10:30:03 2026 GMT
  host: www.freshworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: developers.freshchat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 13:31:52 2026 GMT
  host: api.freshchat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freshchat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freshchat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Freshchat
provider_slug: freshchat
slug: freshchat-domain-security
source_filename: freshchat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freshworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:30:03 2026 GMT\n  hsts: null\n- host: developers.freshchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.freshchat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 13:31:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: freshworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: freshchat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshchat/refs/heads/main/security/freshchat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Messaging
- Live Chat
- Customer Support
- Conversational Engagement
- Omnichannel Messaging
- Chatbots
- Freshworks
---
