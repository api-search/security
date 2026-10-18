---
api_specs:
- filename: checkout-checkout-api-api-openapi.yml
  format: yaml
  label: Checkout Checkout API
  slug: checkout-checkout-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkout/refs/heads/main/openapi/checkout-checkout-api-api-openapi.yml
- filename: checkout-connect-api-openapi.yml
  format: yaml
  label: Checkout Connect API
  slug: checkout-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkout/refs/heads/main/openapi/checkout-connect-api-openapi.yml
- filename: checkout-payments-api-openapi.yml
  format: yaml
  label: Checkout Payments API
  slug: checkout-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkout/refs/heads/main/openapi/checkout-payments-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: checkout.com
  spf: true
hosts:
- cert_expires: Dec 15 11:50:10 2026 GMT
  host: www.checkout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Checkout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Checkout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Checkout
provider_slug: checkout
slug: checkout-domain-security
source_filename: checkout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.checkout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 11:50:10 2026 GMT\n  hsts: false\ndomains:\n- domain: checkout.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkout/refs/heads/main/security/checkout-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Fintech
- E-Commerce
- Global
---
