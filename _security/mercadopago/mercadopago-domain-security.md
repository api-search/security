---
description: ''
domains:
- caa:
  - 0 issue "visa.com"
  - 0 iodef "mailto:domains@mercadolibre.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mercadopago.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:domains@mercadolibre.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mercadopago.com.ar
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.mercadopago.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.mercadopago.com.ar
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: api.mercadopago.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mercadopago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mercado Pago, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mercado Pago
provider_slug: mercadopago
slug: mercadopago-domain-security
source_filename: mercadopago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mercadopago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.mercadopago.com.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.mercadopago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mercadopago.com\n  dnssec: false\n  caa:\n  - 0 issue \"visa.com\"\n  - 0 iodef \"mailto:domains@mercadolibre.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mercadopago.com.ar\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:domains@mercadolibre.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercadopago/refs/heads/main/security/mercadopago-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Checkout
- Subscriptions
- POS
- QR
- SDKs
- Latin America
- Brazil
- Argentina
- Mexico
- Fintech
---
