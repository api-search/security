---
api_specs:
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Checkout API
  slug: geidea-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Direct API
  slug: geidea-direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Tokenization API
  slug: geidea-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
- filename: geidea-openapi.yml
  format: yaml
  label: Geidea Transaction Management API
  slug: geidea-transaction-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/openapi/geidea-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: geidea.net
  spf: true
  spf_record: v=spf1 ip4:193.122.85.214 ip4:178.20.148.109 ip4:176.241.190.146 -all
- dmarc: true
  dmarc_policy: reject
  domain: geidea.ae
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
  cert_subject_o: GEIDEA TECHNOLOGY COMPANY
  host: geidea.net
  hsts: false
  http_status: 302
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 05:29:39 2026 GMT
  cert_issuer: Google Trust Services WE1
  host: docs.geidea.net
  hsts: true
  hsts_max_age: 31536000
  http_status: 302
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
  cert_subject_o: GEIDEA TECHNOLOGY COMPANY
  host: api.ksamerchant.geidea.net
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 401
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 28 23:59:59 2026 GMT
  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
  cert_subject_o: GEIDEA TECHNOLOGY COMPANY
  host: api.merchant.geidea.net
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 401
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 18 23:59:59 2027 GMT
  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
  cert_subject_o: GEIDEA TECHNOLOGY COMPANY
  host: api.geidea.ae
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 204
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geidea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geidea, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Geidea
provider_slug: geidea
slug: geidea-domain-security
source_filename: geidea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geidea.net\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_subject_o: GEIDEA TECHNOLOGY COMPANY\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  http_status: 302\n  hsts: false\n- host: docs.geidea.net\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services WE1\n  cert_expires: Oct  3 05:29:39 2026 GMT\n  http_status: 302\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ksamerchant.geidea.net\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_subject_o: GEIDEA TECHNOLOGY COMPANY\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  http_status: 401\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: api.merchant.geidea.net\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: DigiCert Global G2 TLS RSA SHA256\
  \ 2020 CA1\n  cert_subject_o: GEIDEA TECHNOLOGY COMPANY\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  http_status: 401\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: api.geidea.ae\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  cert_subject_o: GEIDEA TECHNOLOGY COMPANY\n  cert_expires: Jan 18 23:59:59 2027 GMT\n  http_status: 204\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\ndomains:\n- domain: geidea.net\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 ip4:193.122.85.214 ip4:178.20.148.109 ip4:176.241.190.146 -all\n  dmarc: true\n  dmarc_policy: reject\n- domain: geidea.ae\n  dmarc: true\n  dmarc_policy: reject\nnotes: >-\n  All API hosts serve HTTPS with valid DigiCert certificates and enforce HSTS with\n  includeSubDomains; api.geidea.ae additionally sets preload. The unauthenticated\n  API hosts correctly return 401 (KSA, Egypt) or 204\
  \ (UAE ping) without credentials.\n  geidea.net root did not present an HSTS header on its redirect at probe time and\n  no CAA records were observed for geidea.net. api.ksamerchant.geidea.net negotiated\n  TLS 1.2 while the other hosts negotiated TLS 1.3.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geidea/refs/heads/main/security/geidea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Saudi Arabia
- Egypt
- MENA
- mada
- Cards
- POS
- Checkout
- Fintech
---
