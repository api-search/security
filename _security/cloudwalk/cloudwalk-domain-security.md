---
api_specs:
- filename: cloudwalk-infinitepay-checkout-openapi.yml
  format: yaml
  label: InfinitePay Checkout API
  slug: infinitepay-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudwalk/refs/heads/main/openapi/cloudwalk-infinitepay-checkout-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cloudwalk.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: infinitepay.io
  spf: true
hosts:
- cert_expires: Sep 10 16:19:07 2026 GMT
  host: www.cloudwalk.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 08:30:51 2026 GMT
  host: www.infinitepay.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 03:10:30 2026 GMT
  host: api.checkout.infinitepay.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudwalk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudWalk, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CloudWalk
provider_slug: cloudwalk
slug: cloudwalk-domain-security
source_filename: cloudwalk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudwalk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 16:19:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.infinitepay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 08:30:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.checkout.infinitepay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 03:10:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cloudwalk.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: infinitepay.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudwalk/refs/heads/main/security/cloudwalk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Financial Services
- Fintech
- Checkout
- Point of Sale
- Acquiring
- Pix
- Brazil
- Banking
- Webhooks
- Tap to Pay
---
