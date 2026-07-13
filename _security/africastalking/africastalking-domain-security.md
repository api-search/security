---
api_specs:
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking SMS API
  slug: sms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking USSD API
  slug: ussd
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Voice API
  slug: voice
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Airtime API
  slug: airtime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Mobile Data API
  slug: mobile-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
- filename: africastalking-openapi.yml
  format: yaml
  label: Africa's Talking Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/openapi/africastalking-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: africastalking.com
  spf: true
hosts:
- cert_expires: Aug 26 13:41:30 2026 GMT
  host: africastalking.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 04:58:26 2026 GMT
  host: developers.africastalking.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.africastalking.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Africastalking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Africa''s Talking, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Africa's Talking
provider_slug: africastalking
slug: africastalking-domain-security
source_filename: africastalking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: africastalking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 13:41:30 2026 GMT\n  hsts: false\n- host: developers.africastalking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 04:58:26 2026 GMT\n  hsts: false\n- host: api.africastalking.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: africastalking.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/africastalking/refs/heads/main/security/africastalking-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Communications
- SMS
- USSD
- Voice
- Airtime
- Mobile Data
- Payments
- Africa
---
