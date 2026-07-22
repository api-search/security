---
api_specs:
- filename: natwest-account-transaction-openapi.yml
  format: yaml
  label: NatWest Account and Transaction API
  slug: natwest-account-and-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-account-transaction-openapi.yml
- filename: natwest-payment-initiation-openapi.yml
  format: yaml
  label: NatWest Payment Initiation API
  slug: natwest-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-payment-initiation-openapi.yml
- filename: natwest-confirmation-of-funds-openapi.yml
  format: yaml
  label: NatWest Confirmation of Funds API
  slug: natwest-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/openapi/natwest-confirmation-of-funds-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:RBS.Group.PKI.Certificates@rbs.co.uk"
  - 0 issue "digicert.com"
  - 0 issue "quovadisglobal.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: natwest.com
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:RBS.Group.PKI.Certificates@rbs.co.uk"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bankofapis.com
  spf: true
hosts:
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: www.natwest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.bankofapis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: api.sandbox.natwest.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Natwest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NatWest Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NatWest Group
provider_slug: natwest
slug: natwest-domain-security
source_filename: natwest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.natwest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.bankofapis.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sandbox.natwest.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: natwest.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:RBS.Group.PKI.Certificates@rbs.co.uk\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"quovadisglobal.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bankofapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:RBS.Group.PKI.Certificates@rbs.co.uk\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/natwest/refs/heads/main/security/natwest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Open Banking
- Financial Services
- Payments
- PSD2
- FAPI
- Fintech
- Account Information
---
