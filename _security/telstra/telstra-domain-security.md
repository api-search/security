---
api_specs:
- filename: telstra-messaging-api-openapi.yml
  format: yaml
  label: Telstra Messaging API
  slug: telstra-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/openapi/telstra-messaging-api-openapi.yml
- filename: telstra-mobile-number-verification-api-openapi.yml
  format: yaml
  label: Telstra Mobile Number Verification API
  slug: telstra-mobile-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/openapi/telstra-mobile-number-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: telstra.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: telstra.com.au
  spf: true
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: dev.telstra.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: www.telstra.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: tapi.telstra.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Telstra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telstra, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Telstra
provider_slug: telstra
slug: telstra-domain-security
source_filename: telstra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.telstra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: false\n- host: www.telstra.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tapi.telstra.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: telstra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: telstra.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/security/telstra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Telco
- Mobile
- Messaging
- SMS
- MMS
- Networks
- Australia
- Verification
---
