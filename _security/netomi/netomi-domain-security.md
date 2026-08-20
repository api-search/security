---
api_specs:
- filename: netomi-agentdesk-openapi.json
  format: json
  label: Netomi Platform API
  slug: netomi-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netomi/refs/heads/main/openapi/netomi-agentdesk-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netomi.com
  spf: true
hosts:
- cert_expires: Sep 16 06:03:25 2026 GMT
  host: www.netomi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.netomi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 05:23:38 2026 GMT
  host: status.netomi.com
  hsts: true
  hsts_max_age: 31535937
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Netomi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netomi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Netomi
provider_slug: netomi
slug: netomi-domain-security
source_filename: netomi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netomi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:03:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.netomi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\n- host: status.netomi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 05:23:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31535937\ndomains:\n- domain: netomi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netomi/refs/heads/main/security/netomi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Agentic AI
- Customer Experience
- Customer Service
- Customer-Support
- Conversational AI
- Chatbots
- Chat
- Voice
- Telephony
- SDK
- Mobile
---
