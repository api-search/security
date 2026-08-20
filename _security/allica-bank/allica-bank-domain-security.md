---
api_specs:
- filename: allica-bank-account-information-openapi.yaml
  format: yaml
  label: Allica Bank Account and Transaction Information API
  slug: allica-bank-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-account-information-openapi.yaml
- filename: allica-bank-payment-initiation-openapi.yaml
  format: yaml
  label: Allica Bank Payment Initiation API
  slug: allica-bank-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-payment-initiation-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: allica.bank
  spf: true
hosts:
- cert_expires: Sep 23 13:24:04 2026 GMT
  host: www.allica.bank
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: developer.api.ob.allica.bank
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: rs1.api.ob.allica.bank
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Allica Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allica Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Allica Bank
provider_slug: allica-bank
slug: allica-bank-domain-security
source_filename: allica-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allica.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:24:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.api.ob.allica.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rs1.api.ob.allica.bank\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: allica.bank\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/security/allica-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- SME
- Business Banking
- Fintech
---
