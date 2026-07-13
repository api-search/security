---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: heartland.us
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: globalpayments.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.heartland.us
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 23:59:59 2026 GMT
  host: developer.globalpayments.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heartland Payment Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heartland Payment Systems, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Heartland Payment Systems
provider_slug: heartland-payment-systems
slug: heartland-payment-systems-domain-security
source_filename: heartland-payment-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heartland.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\n- host: developer.globalpayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: heartland.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: globalpayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heartland-payment-systems/refs/heads/main/security/heartland-payment-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bill Pay
- Card Present
- Card Not Present
- Ecommerce
- Payment Processing
- Payments
- Payroll
- Point of Sale
- Fortune 1000
---
