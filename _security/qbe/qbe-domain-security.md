---
api_specs:
- filename: qbe-anzo-digital-brokers-openapi.yml
  format: yaml
  label: QBE Australia ANZO Digital Brokers Experience API
  slug: qbe-anzo-digital-brokers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qbe/refs/heads/main/openapi/qbe-anzo-digital-brokers-openapi.yml
- filename: qbe-ctp-switch-service-openapi.yml
  format: yaml
  label: QBE Australia CTP Switch Service
  slug: qbe-ctp-switch-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qbe/refs/heads/main/openapi/qbe-ctp-switch-service-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qbe.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: www.qbe.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: connect.api-au.qbe.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: gateway.api-au.qbe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qbe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QBE Insurance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: QBE Insurance
provider_slug: qbe
slug: qbe-domain-security
source_filename: qbe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qbe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\n- host: connect.api-au.qbe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.api-au.qbe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: qbe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qbe/refs/heads/main/security/qbe-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Insurance
- Australia
- Property and Casualty
- Commercial Insurance
- Underwriting
- Policy Administration
- Quote
- Broker
- Reinsurance
- Carrier
- Partner API
---
