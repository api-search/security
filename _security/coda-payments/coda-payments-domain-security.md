---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coda.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: codapayments.com
  spf: true
hosts:
- cert_expires: Sep  4 05:36:53 2026 GMT
  host: www.coda.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 15:44:25 2026 GMT
  host: docs.coda.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: airtime.codapayments.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coda Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coda Payments, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coda Payments
provider_slug: coda-payments
slug: coda-payments-domain-security
source_filename: coda-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coda.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 05:36:53 2026 GMT\n  hsts: null\n- host: docs.coda.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 15:44:25 2026 GMT\n  hsts: null\n- host: airtime.codapayments.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coda.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: codapayments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coda-payments/refs/heads/main/security/coda-payments-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Merchant of Record
- Gaming
- Digital Goods
- Carrier Billing
- E-Wallets
- Payouts
- Southeast Asia
- Monetization
---
