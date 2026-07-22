---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onepay.com
  spf: true
hosts:
- cert_expires: Oct 13 03:53:48 2026 GMT
  host: www.onepay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onepay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OnePay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OnePay
provider_slug: onepay
slug: onepay-domain-security
source_filename: onepay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.onepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 03:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onepay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onepay/refs/heads/main/security/onepay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Mobile Banking
- Payments
- Consumer Finance
- Credit
- Investing
- Cryptocurrency
- Walmart
---
