---
api_specs:
- filename: kudosity-transmit-message-openapi-original.yml
  format: yaml
  label: Transmit Message API
  slug: transmit-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-transmit-message-openapi-original.yml
- filename: kudosity-transmit-sms-openapi-original.yml
  format: yaml
  label: Transmit SMS API
  slug: transmit-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/openapi/kudosity-transmit-sms-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kudosity.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: transmitmessage.com
  spf: false
hosts:
- cert_expires: Sep 15 02:20:45 2026 GMT
  host: developers.kudosity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: api.transmitmessage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: api.transmitsms.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kudosity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kudosity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kudosity
provider_slug: kudosity
slug: kudosity-domain-security
source_filename: kudosity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.kudosity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:20:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.transmitmessage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\n- host: api.transmitsms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kudosity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: transmitmessage.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kudosity/refs/heads/main/security/kudosity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Messaging
- SMS
- MMS
- RCS
- WhatsApp
- Communications
- CPaaS
- Webhook
- MCP
- agent-native
- Australia
- Notification
- Two-Way Messaging
- Contact Management
---
