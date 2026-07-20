---
api_specs:
- filename: truora-openapi.yml
  format: yaml
  label: Truora Checks API
  slug: truora-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Validators API
  slug: truora-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Digital Identity API
  slug: truora-digital-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
- filename: truora-openapi.yml
  format: yaml
  label: Truora Account API
  slug: truora-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/openapi/truora-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: truora.com
  spf: true
hosts:
- cert_expires: Sep 27 16:01:37 2026 GMT
  host: www.truora.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: dev.truora.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: api.checks.truora.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truora, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Truora
provider_slug: truora
slug: truora-domain-security
source_filename: truora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.truora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:01:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.truora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.checks.truora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: truora.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truora/refs/heads/main/security/truora-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- KYC
- Background Checks
- Fraud Prevention
- LatAm
- WhatsApp
---
