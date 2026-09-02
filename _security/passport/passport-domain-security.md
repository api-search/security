---
api_specs:
- filename: passport-cart-api-openapi.yml
  format: yaml
  label: Passport Cart API
  slug: passport-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-cart-api-openapi.yml
- filename: passport-healthcheck-api-openapi.yml
  format: yaml
  label: Passport Healthcheck API
  slug: passport-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-healthcheck-api-openapi.yml
- filename: passport-order-api-openapi.yml
  format: yaml
  label: Passport Order API
  slug: passport-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-order-api-openapi.yml
- filename: passport-product-price-api-openapi.yml
  format: yaml
  label: Passport Product Price API
  slug: passport-product-price-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-product-price-api-openapi.yml
- filename: passport-rate-api-openapi.yml
  format: yaml
  label: Passport Rate API
  slug: passport-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-rate-api-openapi.yml
- filename: passport-ship-api-openapi.yml
  format: yaml
  label: Passport Ship API
  slug: passport-ship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-ship-api-openapi.yml
- filename: passport-tax-and-duty-api-openapi.yml
  format: yaml
  label: Passport Tax And Duty API
  slug: passport-tax-and-duty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-tax-and-duty-api-openapi.yml
- filename: passport-void-api-openapi.yml
  format: yaml
  label: Passport Void API
  slug: passport-void-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/openapi/passport-void-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: passportglobal.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: passportshipping.com
  spf: true
hosts:
- cert_expires: Jan 16 18:01:54 2027 GMT
  host: passportglobal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 18:01:54 2027 GMT
  host: docs.passportglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 22:34:05 2026 GMT
  host: api.passportshipping.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Passport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Passport, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Passport
provider_slug: passport
slug: passport-domain-security
source_filename: passport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: passportglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 18:01:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.passportglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 18:01:54 2027 GMT\n  hsts: false\n- host: api.passportshipping.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 22:34:05 2026 GMT\n  hsts: null\ndomains:\n- domain: passportglobal.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: passportshipping.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/passport/refs/heads/main/security/passport-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Shipping
- Logistics
- Cross-border eCommerce
- International Shipping
- Customs Compliance
- Landed Cost
- duties-and-taxes
- Parcel Delivery
- E-Commerce
- Merchant of Record
- Trade Compliance
---
