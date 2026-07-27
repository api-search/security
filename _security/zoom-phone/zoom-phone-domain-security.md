---
api_specs:
- filename: zoom-phone-api-openapi.json
  format: json
  label: Zoom Phone API
  slug: zoom-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/openapi/zoom-phone-api-openapi.json
- filename: zoom-phone-webhooks-openapi.json
  format: json
  label: Zoom Phone Webhooks
  slug: zoom-phone-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/openapi/zoom-phone-webhooks-openapi.json
- filename: zoom-phone-number-management-openapi.json
  format: json
  label: Zoom Phone Number Management API
  slug: zoom-phone-number-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/openapi/zoom-phone-number-management-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoom.com
  spf: true
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:security@zoom.us"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zoom.us
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.zoom.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: developers.zoom.us
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: api.zoom.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoom Phone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoom Phone, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zoom Phone
provider_slug: zoom-phone
slug: zoom-phone-domain-security
source_filename: zoom-phone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zoom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.zoom.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: false\n- host: api.zoom.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zoom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zoom.us\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:security@zoom.us\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoom-phone/refs/heads/main/security/zoom-phone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- United States
- UCaaS
- Cloud PBX
- Voice
- VoIP
- SIP
- Messaging
- SMS
- Phone Numbers
- Number Porting
- BYOC
- Carrier Peering
- Contact Center
- Communications
---
