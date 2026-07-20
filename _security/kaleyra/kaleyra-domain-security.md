---
api_specs:
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra SMS API
  slug: kaleyra-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra WhatsApp API
  slug: kaleyra-whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra RCS API
  slug: kaleyra-rcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra Voice API
  slug: kaleyra-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra Verify (OTP) API
  slug: kaleyra-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
- filename: kaleyra-openapi.yml
  format: yaml
  label: Kaleyra Video API
  slug: kaleyra-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/openapi/kaleyra-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kaleyra.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kaleyra.io
  spf: true
hosts:
- cert_expires: Sep 21 08:13:47 2026 GMT
  host: www.kaleyra.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:57:05 2026 GMT
  host: developers.kaleyra.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: api.kaleyra.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kaleyra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaleyra, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kaleyra
provider_slug: kaleyra
slug: kaleyra-domain-security
source_filename: kaleyra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kaleyra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:13:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.kaleyra.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:57:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kaleyra.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kaleyra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kaleyra.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaleyra/refs/heads/main/security/kaleyra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CPaaS
- Messaging
- SMS
- WhatsApp
- Voice
- OTP
- India
---
