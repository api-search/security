---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wearepay.uk
  spf: true
hosts:
- cert_expires: Aug 18 05:31:32 2026 GMT
  host: www.wearepay.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pay Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pay.UK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pay.UK
provider_slug: pay-uk
slug: pay-uk-domain-security
source_filename: pay-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wearepay.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 05:31:32 2026 GMT\n  hsts: null\ndomains:\n- domain: wearepay.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pay-uk/refs/heads/main/security/pay-uk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Payments
- United Kingdom
- Real-Time Payments
- ISO 20022
- Account-to-Account
- Faster Payments
- Direct Debit
- Payment Scheme
- Standards Body
- Confirmation of Payee
---
