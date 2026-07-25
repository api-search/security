---
api_specs:
- filename: sobot-agent-api-openapi.yml
  format: yaml
  label: Sobot Agent API
  slug: sobot-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/openapi/sobot-agent-api-openapi.yml
- filename: sobot-basic-public-service-api-openapi.yml
  format: yaml
  label: Sobot basic-public/service/坐席信息管理 API
  slug: sobot-basic-public-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/openapi/sobot-basic-public-service-api-openapi.yml
- filename: sobot-exts-api-openapi.yml
  format: yaml
  label: Sobot Exts API
  slug: sobot-exts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/openapi/sobot-exts-api-openapi.yml
- filename: sobot-user-api-openapi.yml
  format: yaml
  label: Sobot User API
  slug: sobot-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/openapi/sobot-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sobot.io
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mintlify.com
  spf: true
hosts:
- cert_expires: Aug 22 23:00:12 2026 GMT
  host: docs.sobot.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 02:23:04 2027 GMT
  host: sg.sobot.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: sandbox.mintlify.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sobot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sobot, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sobot
provider_slug: sobot
slug: sobot-domain-security
source_filename: sobot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.sobot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:00:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sg.sobot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 02:23:04 2027 GMT\n  hsts: false\n- host: sandbox.mintlify.com\n  https: false\ndomains:\n- domain: sobot.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: mintlify.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sobot/refs/heads/main/security/sobot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Contact Center
- Customer Service
- Live Chat
- Chatbot
- Voice
- Ticketing
- WhatsApp
- Omnichannel
- Communications
- Artificial Intelligence
---
