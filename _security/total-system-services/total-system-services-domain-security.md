---
api_specs:
- filename: tsys-payment-gateway-openapi.yml
  format: yaml
  label: TSYS Payment Gateway
  slug: tsys-payment-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-system-services/refs/heads/main/openapi/tsys-payment-gateway-openapi.yml
- filename: tsys-issuing-openapi.yml
  format: yaml
  label: TSYS Issuing Platform
  slug: tsys-issuing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-system-services/refs/heads/main/openapi/tsys-issuing-openapi.yml
- filename: tsys-merchant-openapi.yml
  format: yaml
  label: TSYS Merchant Services
  slug: tsys-merchant
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/total-system-services/refs/heads/main/openapi/tsys-merchant-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tsys.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tsysmerchant.com
  spf: false
hosts:
- cert_expires: Sep 14 13:00:26 2026 GMT
  host: www.tsys.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: developers.tsys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: docs.tsysmerchant.com
  https: false
kind: domain-security
layout: security
method: probed
name: Total System Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Total System Services, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Total System Services
provider_slug: total-system-services
slug: total-system-services-domain-security
source_filename: total-system-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tsys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:00:26 2026 GMT\n  hsts: null\n- host: developers.tsys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.tsysmerchant.com\n  https: false\ndomains:\n- domain: tsys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tsysmerchant.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/total-system-services/refs/heads/main/security/total-system-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Processing
- Card Issuing
- Merchant Services
- Fintech
- Financial Services
- Fortune 1000
---
