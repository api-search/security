---
api_specs:
- filename: trulioo-verifications-api-openapi.yml
  format: yaml
  label: Trulioo Verifications API
  slug: trulioo-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-verifications-api-openapi.yml
- filename: trulioo-configuration-api-openapi.yml
  format: yaml
  label: Trulioo Configuration API
  slug: trulioo-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-configuration-api-openapi.yml
- filename: trulioo-connection-api-openapi.yml
  format: yaml
  label: Trulioo Connection API
  slug: trulioo-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-connection-api-openapi.yml
- filename: trulioo-business-verification-api-openapi.yml
  format: yaml
  label: Trulioo Business Verification API
  slug: trulioo-business-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-business-verification-api-openapi.yml
- filename: trulioo-person-fraud-api-openapi.yml
  format: yaml
  label: Trulioo Person Fraud API
  slug: trulioo-person-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-person-fraud-api-openapi.yml
- filename: trulioo-document-verification-api-openapi.yml
  format: yaml
  label: Trulioo Identity Document Verification API
  slug: trulioo-document-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-document-verification-api-openapi.yml
- filename: trulioo-platform-api-openapi.yml
  format: yaml
  label: Trulioo Platform API
  slug: trulioo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/openapi/trulioo-platform-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trulioo.com
  spf: true
hosts:
- cert_expires: Aug 20 13:23:51 2026 GMT
  host: www.trulioo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 15:12:04 2026 GMT
  host: developer.trulioo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 23:59:59 2026 GMT
  host: api.trulioo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trulioo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trulioo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trulioo
provider_slug: trulioo
slug: trulioo-domain-security
source_filename: trulioo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trulioo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 13:23:51 2026 GMT\n  hsts: false\n- host: developer.trulioo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.trulioo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trulioo.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trulioo/refs/heads/main/security/trulioo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- KYC
- KYB
- AML
- Watchlist Screening
- Biometrics
- Document Verification
- Fraud Prevention
- Compliance
- Global Identity
---
