---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bridgtheapp.com
  spf: true
hosts:
- host: bridgtheapp.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''bridgtheapp'
kind: domain-security
layout: security
method: probed
name: Bridg Payment Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bridg Payment Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bridg Payment Solutions
provider_slug: bridg-payment-solutions
slug: bridg-payment-solutions-domain-security
source_filename: bridg-payment-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bridgtheapp.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''bridgtheapp'\n  hsts: null\ndomains:\n- domain: bridgtheapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridg-payment-solutions/refs/heads/main/security/bridg-payment-solutions-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Payments
- Fintech
- Mobile Payments
- Point of Sale
- Bluetooth
- Offline Payments
- Digital Wallet
- UAE
---
