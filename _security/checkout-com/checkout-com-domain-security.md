---
api_specs:
- filename: checkout-com-customers-api-openapi.yml
  format: yaml
  label: Checkout.com Customers API
  slug: checkout-com-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkout-com/refs/heads/main/openapi/checkout-com-customers-api-openapi.yml
- filename: checkout-com-instruments-api-openapi.yml
  format: yaml
  label: Checkout.com Instruments API
  slug: checkout-com-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkout-com/refs/heads/main/openapi/checkout-com-instruments-api-openapi.yml
- filename: checkout-com-payments-api-openapi.yml
  format: yaml
  label: Checkout.com Payments API
  slug: checkout-com-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkout-com/refs/heads/main/openapi/checkout-com-payments-api-openapi.yml
- filename: checkout-com-tokens-api-openapi.yml
  format: yaml
  label: Checkout.com Tokens API
  slug: checkout-com-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkout-com/refs/heads/main/openapi/checkout-com-tokens-api-openapi.yml
- filename: checkout-com-workflows-api-openapi.yml
  format: yaml
  label: Checkout.com Workflows API
  slug: checkout-com-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkout-com/refs/heads/main/openapi/checkout-com-workflows-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: checkout.com
  spf: true
hosts:
- cert_expires: Sep 22 16:08:55 2026 GMT
  host: www.checkout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  1 13:58:13 2026 GMT
  host: api-reference.checkout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: api.checkout.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Checkout Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Checkout.com, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Checkout.com
provider_slug: checkout-com
slug: checkout-com-domain-security
source_filename: checkout-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checkout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 16:08:55 2026 GMT\n  hsts: false\n- host: api-reference.checkout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 13:58:13 2026 GMT\n  hsts: false\n- host: api.checkout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: checkout.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkout-com/refs/heads/main/security/checkout-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fintech
- Payments
- Cards
- Acquiring
- Cross-Border
---
