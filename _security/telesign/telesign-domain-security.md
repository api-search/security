---
api_specs:
- filename: telesign-fraud-scoring-api-openapi.yml
  format: yaml
  label: Telesign Fraud Scoring API
  slug: telesign-fraud-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-fraud-scoring-api-openapi.yml
- filename: telesign-messaging-api-openapi.yml
  format: yaml
  label: Telesign Messaging API
  slug: telesign-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-messaging-api-openapi.yml
- filename: telesign-phone-intelligence-api-openapi.yml
  format: yaml
  label: Telesign Phone Intelligence API
  slug: telesign-phone-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-phone-intelligence-api-openapi.yml
- filename: telesign-verification-api-openapi.yml
  format: yaml
  label: Telesign Verification API
  slug: telesign-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: telesign.com
  spf: true
hosts:
- cert_expires: Sep 15 01:48:07 2026 GMT
  host: www.telesign.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 07:42:41 2026 GMT
  host: developer.telesign.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: rest-ww.telesign.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telesign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telesign, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Telesign
provider_slug: telesign
slug: telesign-domain-security
source_filename: telesign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.telesign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:48:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.telesign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 07:42:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rest-ww.telesign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: telesign.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/security/telesign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Communications
- Fraud Prevention
- Phone Intelligence
- SMS
- Verification
---
