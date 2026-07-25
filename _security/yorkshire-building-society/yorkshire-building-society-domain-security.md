---
api_specs:
- filename: yorkshire-building-society-account-information-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Account Information API
  slug: ybs-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-account-information-api-openapi.yaml
- filename: yorkshire-building-society-payment-initiation-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Payment Initiation API
  slug: ybs-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-payment-initiation-api-openapi.yaml
- filename: yorkshire-building-society-confirmation-of-funds-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Confirmation of Funds API
  slug: ybs-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-confirmation-of-funds-api-openapi.yaml
- filename: yorkshire-building-society-event-subscriptions-api-openapi.yaml
  format: yaml
  label: Yorkshire Building Society Event Subscriptions API
  slug: ybs-event-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/openapi/yorkshire-building-society-event-subscriptions-api-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ybs.co.uk
  spf: true
hosts:
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: www.ybs.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 13:55:54 2026 GMT
  host: developers.ybs.co.uk
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: ob-ybs.api.ybs.co.uk
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate in certificate chain (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Yorkshire Building Society Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yorkshire Building Society, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yorkshire Building Society
provider_slug: yorkshire-building-society
slug: yorkshire-building-society-domain-security
source_filename: yorkshire-building-society-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ybs.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.ybs.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:55:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: ob-ybs.api.ybs.co.uk\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    in certificate chain (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: ybs.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yorkshire-building-society/refs/heads/main/security/yorkshire-building-society-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Building Society
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- Fintech
---
