---
api_specs:
- filename: giftbit-openapi.yml
  format: yaml
  label: Giftbit API
  slug: giftbit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/openapi/giftbit-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:bugs@giftbit.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: giftbit.com
  spf: true
hosts:
- cert_expires: Sep  2 22:29:53 2026 GMT
  host: www.giftbit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:36:56 2026 GMT
  host: api.giftbit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 05:02:58 2026 GMT
  host: api-testbed.giftbit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Giftbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Giftbit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Giftbit
provider_slug: giftbit
slug: giftbit-domain-security
source_filename: giftbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.giftbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 22:29:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.giftbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:36:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-testbed.giftbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:02:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: giftbit.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:bugs@giftbit.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/giftbit/refs/heads/main/security/giftbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gift Cards
- Digital Rewards
- Incentives
- Payments
- Reward Distribution
- Prepaid Cards
---
