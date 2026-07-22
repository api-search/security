---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paynearme.com
  spf: true
hosts:
- cert_expires: Oct 12 10:43:15 2026 GMT
  host: www.paynearme.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paynearme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayNearMe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PayNearMe
provider_slug: paynearme
slug: paynearme-domain-security
source_filename: paynearme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paynearme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 10:43:15 2026 GMT\n  hsts: null\ndomains:\n- domain: paynearme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paynearme/refs/heads/main/security/paynearme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Payments
- Billing
- ACH
- Cash Payments
- Digital Wallets
- Lending
- iGaming
- Webhooks
---
