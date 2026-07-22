---
api_specs:
- filename: zavu-openapi-original.json
  format: json
  label: Zavu Unified Messaging Layer API
  slug: zavu-unified-messaging-layer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zavu/refs/heads/main/openapi/zavu-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: zavu.dev
  spf: false
hosts:
- cert_expires: Aug 25 15:26:31 2026 GMT
  host: zavu.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 01:25:57 2026 GMT
  host: api.zavu.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zavu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zavu, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Zavu
provider_slug: zavu
slug: zavu-domain-security
source_filename: zavu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zavu.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:26:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.zavu.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 01:25:57 2026 GMT\n  hsts: null\ndomains:\n- domain: zavu.dev\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zavu/refs/heads/main/security/zavu-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Messaging
- SMS
- WhatsApp
- Email
- Voice
- Communications
- CPaaS
- Webhooks
- AI Agents
---
