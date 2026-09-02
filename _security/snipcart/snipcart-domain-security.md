---
api_specs:
- filename: snipcart-abandonedcarts-api-openapi.yml
  format: yaml
  label: Snipcart AbandonedCarts API
  slug: snipcart-abandonedcarts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-abandonedcarts-api-openapi.yml
- filename: snipcart-customers-api-openapi.yml
  format: yaml
  label: Snipcart Customers API
  slug: snipcart-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-customers-api-openapi.yml
- filename: snipcart-discounts-api-openapi.yml
  format: yaml
  label: Snipcart Discounts API
  slug: snipcart-discounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-discounts-api-openapi.yml
- filename: snipcart-domains-api-openapi.yml
  format: yaml
  label: Snipcart Domains API
  slug: snipcart-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-domains-api-openapi.yml
- filename: snipcart-notifications-api-openapi.yml
  format: yaml
  label: Snipcart Notifications API
  slug: snipcart-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-notifications-api-openapi.yml
- filename: snipcart-orders-api-openapi.yml
  format: yaml
  label: Snipcart Orders API
  slug: snipcart-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-orders-api-openapi.yml
- filename: snipcart-products-api-openapi.yml
  format: yaml
  label: Snipcart Products API
  slug: snipcart-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-products-api-openapi.yml
- filename: snipcart-refunds-api-openapi.yml
  format: yaml
  label: Snipcart Refunds API
  slug: snipcart-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-refunds-api-openapi.yml
- filename: snipcart-usersessions-api-openapi.yml
  format: yaml
  label: Snipcart UserSessions API
  slug: snipcart-usersessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/openapi/snipcart-usersessions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: snipcart.com
  spf: true
hosts:
- cert_expires: Sep 10 09:23:56 2026 GMT
  host: snipcart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 16:53:56 2026 GMT
  host: docs.snipcart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: app.snipcart.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snipcart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snipcart, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Snipcart
provider_slug: snipcart
slug: snipcart-domain-security
source_filename: snipcart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snipcart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:23:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.snipcart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 16:53:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.snipcart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: snipcart.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snipcart/refs/heads/main/security/snipcart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Shopping Cart
- Order
- Product
- Payments
- Webhook
- Headless Commerce
- JAMstack
---
