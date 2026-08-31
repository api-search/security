---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theyeeld.com
  spf: true
hosts:
- cert_expires: Sep 29 03:31:40 2026 GMT
  host: theyeeld.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: docs.theyeeld.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: api.theyeeld.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Yeeld Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yeeld, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yeeld
provider_slug: yeeld
slug: yeeld-domain-security
source_filename: yeeld-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts; theyeeld.com (the marketing/apex host) re-probed\n  by hand 2026-08-28 and merged back after the humanURL moved to docs.theyeeld.com\nhosts:\n- host: theyeeld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:31:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.theyeeld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\n- host: api.theyeeld.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: theyeeld.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yeeld/refs/heads/main/security/yeeld-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Surcharging
- Credit Cards
- Compliance
- Stripe
- Checkout
- Fintech
- Payment Consulting
---
