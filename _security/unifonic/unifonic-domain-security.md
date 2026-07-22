---
api_specs:
- filename: unifonic-sms-openapi-original.json
  format: json
  label: Unifonic SMS API
  slug: unifonic-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unifonic/refs/heads/main/openapi/unifonic-sms-openapi-original.json
- filename: unifonic-authenticate-openapi-original.json
  format: json
  label: Unifonic Authenticate API
  slug: unifonic-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unifonic/refs/heads/main/openapi/unifonic-authenticate-openapi-original.json
- filename: unifonic-voice-openapi-original.json
  format: json
  label: Unifonic Voice APIs
  slug: unifonic-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unifonic/refs/heads/main/openapi/unifonic-voice-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: unifonic.com
  spf: true
hosts:
- cert_expires: Aug 29 09:16:16 2026 GMT
  host: www.unifonic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 19:15:12 2026 GMT
  host: docs.unifonic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: el.cloud.unifonic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Unifonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unifonic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Unifonic
provider_slug: unifonic
slug: unifonic-domain-security
source_filename: unifonic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unifonic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 09:16:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.unifonic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 19:15:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: el.cloud.unifonic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unifonic.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unifonic/refs/heads/main/security/unifonic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- CPaaS
- Messaging
- SMS
- WhatsApp
- Voice
- Push Notifications
- OTP
- Customer Engagement
- Saudi Arabia
---
