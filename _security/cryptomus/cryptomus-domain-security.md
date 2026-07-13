---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Cryptomus Merchant Payment API
  slug: cryptomus-merchant-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cryptomus.com
  spf: true
hosts:
- cert_expires: Sep 30 14:50:35 2026 GMT
  host: cryptomus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:50:35 2026 GMT
  host: doc.cryptomus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 14:50:35 2026 GMT
  host: api.cryptomus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cryptomus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cryptomus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cryptomus
provider_slug: cryptomus
slug: cryptomus-domain-security
source_filename: cryptomus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cryptomus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:50:35 2026 GMT\n  hsts: false\n- host: doc.cryptomus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:50:35 2026 GMT\n  hsts: false\n- host: api.cryptomus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:50:35 2026 GMT\n  hsts: false\ndomains:\n- domain: cryptomus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptomus/refs/heads/main/security/cryptomus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cryptocurrency
- Payments
- Invoices
- Payouts
- Exchange Rates
- Crypto Gateway
---
