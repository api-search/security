---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uala.com.ar
  spf: true
hosts:
- cert_expires: Oct  1 20:17:19 2026 GMT
  host: www.uala.com.ar
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ualá, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ualá
provider_slug: uala
slug: uala-domain-security
source_filename: uala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uala.com.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:17:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uala.com.ar\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uala/refs/heads/main/security/uala-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Neobank
- Digital Banking
- Prepaid Card
- Mastercard
- Payments
- Lending
- Personal Loans
- Investing
- Brokerage
- Insurance
- Point Of Sale
- Merchant Acquiring
- Payment Links
- Latin America
- Argentina
- Mexico
- Colombia
- Financial Inclusion
---
