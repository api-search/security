---
api_specs:
- filename: manychat-page-api-openapi.yml
  format: yaml
  label: ManyChat Page API
  slug: manychat-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/openapi/manychat-page-api-openapi.yml
- filename: manychat-sending-api-openapi.yml
  format: yaml
  label: ManyChat Sending API
  slug: manychat-sending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/openapi/manychat-sending-api-openapi.yml
- filename: manychat-subscriber-api-openapi.yml
  format: yaml
  label: ManyChat Subscriber API
  slug: manychat-subscriber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/openapi/manychat-subscriber-api-openapi.yml
- filename: manychat-template-api-openapi.yml
  format: yaml
  label: ManyChat Template API
  slug: manychat-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/openapi/manychat-template-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "usertrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: manychat.com
  spf: true
hosts:
- cert_expires: Oct 12 17:16:43 2026 GMT
  host: manychat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.manychat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Manychat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ManyChat, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ManyChat
provider_slug: manychat
slug: manychat-domain-security
source_filename: manychat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manychat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 17:16:43 2026 GMT\n  hsts: null\n- host: api.manychat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: manychat.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"usertrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manychat/refs/heads/main/security/manychat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Chat Marketing
- Messenger Marketing
- Conversational Commerce
- Marketing Automation
- Instagram
- WhatsApp
- Facebook Messenger
- SMS
- Chatbots
- Customer Engagement
- Automation
---
