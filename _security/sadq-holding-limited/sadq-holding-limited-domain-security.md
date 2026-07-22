---
api_specs:
- filename: sadq-holding-limited-openapi-original.json
  format: json
  label: Sadq Integration API
  slug: sadq-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  dmarc: false
  dnssec: false
  domain: sadq-sa.com
  spf: false
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sadq.sa
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: sadq-sa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: api.sadq.sa
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: sandbox-api.sadq-sa.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sadq Holding Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sadq Holding Limited, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sadq Holding Limited
provider_slug: sadq-holding-limited
slug: sadq-holding-limited-domain-security
source_filename: sadq-holding-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sadq-sa.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sadq.sa\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox-api.sadq-sa.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sadq-sa.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: false\n  dmarc: false\n- domain: sadq.sa\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/security/sadq-holding-limited-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- E-Signature
- Digital Signature
- Identity
- KYB
- Document Management
- Saudi Arabia
- Nafath
- Webhooks
- Agent Ready
---
