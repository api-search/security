---
api_specs:
- filename: spree-store-api.yaml
  format: yaml
  label: Spree Store API
  slug: spree-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree/refs/heads/main/openapi/spree-store-api.yaml
- filename: spree-admin-api.yaml
  format: yaml
  label: Spree Admin API
  slug: spree-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree/refs/heads/main/openapi/spree-admin-api.yaml
- filename: spree-storefront-api.yaml
  format: yaml
  label: Spree Storefront API
  slug: spree-storefront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree/refs/heads/main/openapi/spree-storefront-api.yaml
- filename: spree-platform-api.yaml
  format: yaml
  label: Spree Platform API
  slug: spree-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spree/refs/heads/main/openapi/spree-platform-api.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spreecommerce.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yourdomain.com
  spf: true
hosts:
- cert_expires: Sep  2 20:24:06 2026 GMT
  host: spreecommerce.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: yourdomain.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''yourdomain.'
- cert_expires: Aug 31 06:42:20 2026 GMT
  host: demo.spreecommerce.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spree Commerce, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Spree Commerce
provider_slug: spree
slug: spree-domain-security
source_filename: spree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spreecommerce.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:24:06 2026 GMT\n  hsts: false\n- host: yourdomain.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''yourdomain.'\n  hsts: null\n- host: demo.spreecommerce.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 06:42:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: spreecommerce.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: yourdomain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spree/refs/heads/main/security/spree-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Headless Commerce
- Products
- Orders
- Inventory
- Payments
- Promotions
- Open Source
- Ruby on Rails
---
