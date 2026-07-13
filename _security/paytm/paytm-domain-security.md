---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paytm.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "geotrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: paytm.in
  spf: true
hosts:
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: business.paytm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: securegw.paytm.in
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: securegw-stage.paytm.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paytm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paytm, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paytm
provider_slug: paytm
slug: paytm-domain-security
source_filename: paytm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: business.paytm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: null\n- host: securegw.paytm.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\n- host: securegw-stage.paytm.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: paytm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: paytm.in\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"geotrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paytm/refs/heads/main/security/paytm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- Payment Gateway
- UPI
- Payouts
- Subscriptions
- Refunds
- Settlement
- QR
- EDC
- Fintech
- India
---
