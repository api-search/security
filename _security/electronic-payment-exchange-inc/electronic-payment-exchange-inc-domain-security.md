---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: north.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: epx.com
  spf: true
hosts:
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: developer.north.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: secure.epx.com
  https: false
kind: domain-security
layout: security
method: probed
name: Electronic Payment Exchange Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electronic payment Exchange Inc, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Electronic payment Exchange Inc
provider_slug: electronic-payment-exchange-inc
slug: electronic-payment-exchange-inc-domain-security
source_filename: electronic-payment-exchange-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.north.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: false\n- host: secure.epx.com\n  https: false\ndomains:\n- domain: north.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: epx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electronic-payment-exchange-inc/refs/heads/main/security/electronic-payment-exchange-inc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Payment Processing
- Merchant Acquiring
- Payment Gateway
- Tokenization
- Credit Card Processing
- ACH
- Fintech
---
