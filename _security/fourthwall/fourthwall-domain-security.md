---
api_specs:
- filename: fourthwall-collections-api-openapi.yml
  format: yaml
  label: Fourthwall Collections API
  slug: fourthwall-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-collections-api-openapi.yml
- filename: fourthwall-gifting-api-openapi.yml
  format: yaml
  label: Fourthwall Gifting API
  slug: fourthwall-gifting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-gifting-api-openapi.yml
- filename: fourthwall-giveaways-api-openapi.yml
  format: yaml
  label: Fourthwall Giveaways API
  slug: fourthwall-giveaways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-giveaways-api-openapi.yml
- filename: fourthwall-memberships-api-openapi.yml
  format: yaml
  label: Fourthwall Memberships API
  slug: fourthwall-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-memberships-api-openapi.yml
- filename: fourthwall-orders-api-openapi.yml
  format: yaml
  label: Fourthwall Orders API
  slug: fourthwall-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-orders-api-openapi.yml
- filename: fourthwall-products-api-openapi.yml
  format: yaml
  label: Fourthwall Products API
  slug: fourthwall-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-products-api-openapi.yml
- filename: fourthwall-promotions-api-openapi.yml
  format: yaml
  label: Fourthwall Promotions API
  slug: fourthwall-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-promotions-api-openapi.yml
- filename: fourthwall-storefront-carts-api-openapi.yml
  format: yaml
  label: Fourthwall Storefront Carts API
  slug: fourthwall-storefront-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-storefront-carts-api-openapi.yml
- filename: fourthwall-storefront-collections-api-openapi.yml
  format: yaml
  label: Fourthwall Storefront Collections API
  slug: fourthwall-storefront-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-storefront-collections-api-openapi.yml
- filename: fourthwall-storefront-products-api-openapi.yml
  format: yaml
  label: Fourthwall Storefront Products API
  slug: fourthwall-storefront-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-storefront-products-api-openapi.yml
- filename: fourthwall-storefront-shop-api-openapi.yml
  format: yaml
  label: Fourthwall Storefront Shop API
  slug: fourthwall-storefront-shop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-storefront-shop-api-openapi.yml
- filename: fourthwall-webhooks-api-openapi.yml
  format: yaml
  label: Fourthwall Webhooks API
  slug: fourthwall-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/openapi/fourthwall-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fourthwall.com
  spf: true
hosts:
- cert_expires: Sep  1 17:06:05 2026 GMT
  host: fourthwall.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 12:46:50 2026 GMT
  host: docs.fourthwall.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 17:06:05 2026 GMT
  host: storefront-api.fourthwall.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fourthwall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fourthwall, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fourthwall
provider_slug: fourthwall
slug: fourthwall-domain-security
source_filename: fourthwall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fourthwall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:06:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.fourthwall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 12:46:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: storefront-api.fourthwall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:06:05 2026 GMT\n  hsts: null\ndomains:\n- domain: fourthwall.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fourthwall/refs/heads/main/security/fourthwall-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Creator Commerce
- E-Commerce
- Merch
- Storefront
- Memberships
- Donations
- Print on Demand
---
