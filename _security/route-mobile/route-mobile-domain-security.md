---
api_specs:
- filename: route-mobile-sms.yml
  format: yaml
  label: Route Mobile SMS API
  slug: route-mobile-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-sms.yml
- filename: route-mobile-whatsapp-business.yml
  format: yaml
  label: Route Mobile WhatsApp Business API
  slug: route-mobile-whatsapp-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-whatsapp-business.yml
- filename: route-mobile-rcs.yml
  format: yaml
  label: Route Mobile RCS Business Messaging API
  slug: route-mobile-rcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-rcs.yml
- filename: route-mobile-viber.yml
  format: yaml
  label: Route Mobile Viber Business Messages API
  slug: route-mobile-viber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-viber.yml
- filename: route-mobile-sendclean-email.yml
  format: yaml
  label: SendClean Email API
  slug: sendclean-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/openapi/route-mobile-sendclean-email.yml
- filename: Enterprise-Voice-2.0-APIs
  format: yaml
  label: Route Mobile Enterprise Voice 2.0 API
  slug: route-mobile-enterprise-voice-api
  spec_type: Postman
  url: https://github.com/routemobile/Enterprise-Voice-2.0-APIs
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: routemobile.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rmlconnect.net
  spf: false
hosts:
- cert_expires: Dec 28 11:28:00 2026 GMT
  host: routemobile.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 23 11:11:55 2026 GMT
  host: developer.rmlconnect.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 06:10:13 2026 GMT
  host: api.rmlconnect.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Route Mobile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Route Mobile, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Route Mobile
provider_slug: route-mobile
slug: route-mobile-domain-security
source_filename: route-mobile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: routemobile.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 11:28:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.rmlconnect.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 11:11:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rmlconnect.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 06:10:13 2026 GMT\n  hsts: null\ndomains:\n- domain: routemobile.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: rmlconnect.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/route-mobile/refs/heads/main/security/route-mobile-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Telecommunications
- India
- CPaaS
- Messaging
- SMS
- A2P Messaging
- WhatsApp Business
- RCS
- Voice
- Email
- Identity Verification
- OTP
- Aggregator
---
