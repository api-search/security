---
api_specs:
- filename: woocommerce-rest-api-openapi.yml
  format: yaml
  label: WooCommerce REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woocommerce/refs/heads/main/openapi/woocommerce-rest-api-openapi.yml
- filename: woocommerce-store-api-openapi.yml
  format: yaml
  label: WooCommerce Store API
  slug: store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woocommerce/refs/heads/main/openapi/woocommerce-store-api-openapi.yml
- filename: woocommerce-webhooks-asyncapi.yml
  format: yaml
  label: WooCommerce Webhook Events
  slug: webhook-events
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/woocommerce/refs/heads/main/asyncapi/woocommerce-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: woocommerce.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: woographql.com
  spf: false
hosts:
- cert_expires: Aug 31 14:35:28 2026 GMT
  host: woocommerce.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 22:49:54 2026 GMT
  host: developer.woocommerce.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 16:19:37 2026 GMT
  host: woographql.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Woocommerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WooCommerce, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WooCommerce
provider_slug: woocommerce
slug: woocommerce-domain-security
source_filename: woocommerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: woocommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 14:35:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.woocommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 22:49:54 2026 GMT\n  hsts: false\n- host: woographql.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 16:19:37 2026 GMT\n  hsts: false\ndomains:\n- domain: woocommerce.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: woographql.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woocommerce/refs/heads/main/security/woocommerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eCommerce
- Open Source
- Orders
- Products
- WordPress
---
