---
api_specs:
- filename: subbly-openapi.yml
  format: yaml
  label: Subbly Products API
  slug: subbly-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subbly/refs/heads/main/openapi/subbly-openapi.yml
- filename: subbly-openapi.yml
  format: yaml
  label: Subbly Subscriptions API
  slug: subbly-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subbly/refs/heads/main/openapi/subbly-openapi.yml
- filename: subbly-openapi.yml
  format: yaml
  label: Subbly Customers API
  slug: subbly-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subbly/refs/heads/main/openapi/subbly-openapi.yml
- filename: subbly-openapi.yml
  format: yaml
  label: Subbly Cart and Checkout API
  slug: subbly-cart-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/subbly/refs/heads/main/openapi/subbly-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: subbly.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: subbly.dev
  spf: true
hosts:
- cert_expires: Aug 14 03:01:14 2026 GMT
  host: www.subbly.co
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 04:35:12 2026 GMT
  host: docs.subbly.dev
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 04:16:34 2026 GMT
  host: www.subbly.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Subbly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Subbly, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Subbly
provider_slug: subbly
slug: subbly-domain-security
source_filename: subbly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.subbly.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:01:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: docs.subbly.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 04:35:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: www.subbly.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:16:34 2026 GMT\n  hsts: false\ndomains:\n- domain: subbly.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: subbly.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subbly/refs/heads/main/security/subbly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Subscriptions
- Subscription Commerce
- Ecommerce
- Subscription Box
- Recurring Billing
- Headless Commerce
- SDK
- Webhooks
---
