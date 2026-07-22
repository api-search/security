---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paycargo.com
  spf: true
hosts:
- cert_expires: Sep 15 11:38:27 2026 GMT
  host: paycargo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: api.paycargo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paycargo Llc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayCargo, LLC, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PayCargo, LLC
provider_slug: paycargo-llc
slug: paycargo-llc-domain-security
source_filename: paycargo-llc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paycargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:38:27 2026 GMT\n  hsts: false\n- host: api.paycargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: paycargo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paycargo-llc/refs/heads/main/security/paycargo-llc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Freight
- Logistics
- Supply Chain
- Fintech
- Accounts Payable
- Shipping
---
