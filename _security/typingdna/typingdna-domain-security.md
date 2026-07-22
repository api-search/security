---
api_specs:
- filename: typingdna-authentication-api-openapi-original.json
  format: json
  label: TypingDNA Authentication API
  slug: typingdna-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typingdna/refs/heads/main/openapi/typingdna-authentication-api-openapi-original.json
- filename: typingdna-verify-2fa-openapi.json
  format: json
  label: TypingDNA Verify 2FA API
  slug: typingdna-verify-2fa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typingdna/refs/heads/main/openapi/typingdna-verify-2fa-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: typingdna.com
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: typingdna.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: api.typingdna.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: verify.typingdna.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Typingdna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TypingDNA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TypingDNA
provider_slug: typingdna
slug: typingdna-domain-security
source_filename: typingdna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: typingdna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.typingdna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\n- host: verify.typingdna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: typingdna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typingdna/refs/heads/main/security/typingdna-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Authentication
- Biometrics
- Typing Biometrics
- Two-Factor Authentication
- Identity
- Security
- Fraud Prevention
---
