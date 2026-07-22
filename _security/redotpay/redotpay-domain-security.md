---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: redotpay.com
  spf: true
hosts:
- cert_expires: Sep 30 07:08:09 2026 GMT
  host: www.redotpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 07:08:09 2026 GMT
  host: apiv2.redotpay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redotpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redotpay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Redotpay
provider_slug: redotpay
slug: redotpay-domain-security
source_filename: redotpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redotpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 07:08:09 2026 GMT\n  hsts: null\n- host: apiv2.redotpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 07:08:09 2026 GMT\n  hsts: null\ndomains:\n- domain: redotpay.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redotpay/refs/heads/main/security/redotpay-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Payments
- Fintech
- Stablecoin
- Cryptocurrency
- Wallet
- Agentic Payments
- Machine Payments Protocol
- x402
- OAuth
---
