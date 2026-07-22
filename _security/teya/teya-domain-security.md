---
api_specs:
- filename: teya-online-payments-openapi.yaml
  format: yaml
  label: Teya Online Payments API
  slug: teya-online-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-online-payments-openapi.yaml
- filename: teya-payments-openapi.yaml
  format: yaml
  label: Teya Payments Gateway API
  slug: teya-payments-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-payments-openapi.yaml
- filename: teya-poslink-openapi.json
  format: json
  label: Teya POSLink API
  slug: teya-poslink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-poslink-openapi.json
- filename: teya-fx-openapi.yaml
  format: yaml
  label: Teya FX (DCC) API
  slug: teya-fx-dcc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-fx-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: saltpay.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teya.com
  spf: true
hosts:
- cert_expires: Oct  7 04:54:28 2026 GMT
  host: www.saltpay.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: api.teya.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.teya.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teya, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Teya
provider_slug: teya
slug: teya-domain-security
source_filename: teya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saltpay.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:54:28 2026 GMT\n  hsts: null\n- host: api.teya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\n- host: api.teya.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: saltpay.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: teya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/security/teya-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Payment Processing
- Card Acquiring
- Online Payments
- Point of Sale
- E-commerce
- Fintech
- Merchant Services
- Europe
---
