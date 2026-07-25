---
api_specs:
- filename: c-hoare-and-co-account-and-transaction-api-openapi.yml
  format: yaml
  label: C. Hoare & Co. Account and Transaction Information API
  slug: c-hoare-and-co-account-and-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/c-hoare-and-co/refs/heads/main/openapi/c-hoare-and-co-account-and-transaction-api-openapi.yml
- filename: c-hoare-and-co-payment-initiation-api-openapi.yml
  format: yaml
  label: C. Hoare & Co. Payment Initiation API
  slug: c-hoare-and-co-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/c-hoare-and-co/refs/heads/main/openapi/c-hoare-and-co-payment-initiation-api-openapi.yml
- filename: c-hoare-and-co-dynamic-client-registration-api-openapi.yml
  format: yaml
  label: C. Hoare & Co. Dynamic Client Registration API
  slug: c-hoare-and-co-dynamic-client-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/c-hoare-and-co/refs/heads/main/openapi/c-hoare-and-co-dynamic-client-registration-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hoaresbank.co.uk
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: www.hoaresbank.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: developer.hoaresbank.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.hoaresbank.co.uk
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: C Hoare And Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for C. Hoare & Co., probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: C. Hoare & Co.
provider_slug: c-hoare-and-co
slug: c-hoare-and-co-domain-security
source_filename: c-hoare-and-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hoaresbank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.hoaresbank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\n- host: api.hoaresbank.co.uk\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: hoaresbank.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/c-hoare-and-co/refs/heads/main/security/c-hoare-and-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Private Bank
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
---
