---
api_specs:
- filename: api-gateway.yml
  format: yaml
  label: HiPay Payment Gateway API
  slug: hipay-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/api-gateway.yml
- filename: gateway.yaml
  format: yaml
  label: HiPay Enterprise Gateway API
  slug: hipay-enterprise-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/gateway.yaml
- filename: hpayment.yaml
  format: yaml
  label: HiPay Enterprise HostedPage API
  slug: hipay-enterprise-hostedpage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/hpayment.yaml
- filename: settlement.yaml
  format: yaml
  label: HiPay Enterprise Finance API
  slug: hipay-enterprise-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/settlement.yaml
- filename: tokenization.yaml
  format: yaml
  label: HiPay Enterprise Tokenization API
  slug: hipay-enterprise-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/tokenization.yaml
- filename: applepay-web.yaml
  format: yaml
  label: HiPay Apple Pay Web API
  slug: hipay-apple-pay-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/applepay-web.yaml
- filename: pos_api.yaml
  format: yaml
  label: HiPay POS API
  slug: hipay-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/omnichannel/pos_api.yaml
- filename: omnichannel.yaml
  format: yaml
  label: HiPay Omnichannel Gateway API
  slug: hipay-omnichannel-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/omnichannel/omnichannel.yaml
- filename: marketplace.yaml
  format: yaml
  label: HiPay Marketplace API
  slug: hipay-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/marketplace/marketplace.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hipay.com
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: developer.hipay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: hipay.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: api-gateway.hipay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hipay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HiPay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HiPay
provider_slug: hipay
slug: hipay-domain-security
source_filename: hipay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.hipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: hipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api-gateway.hipay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: hipay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/security/hipay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Fintech
- Europe
- Omnichannel
- Point of Sale
- Fraud Prevention
- Tokenization
- Marketplace
---
