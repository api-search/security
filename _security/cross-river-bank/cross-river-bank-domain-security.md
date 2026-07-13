---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: crossriver.com
  spf: true
hosts:
- cert_expires: Aug 24 04:15:37 2026 GMT
  host: www.crossriver.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 02:59:58 2026 GMT
  host: docs.crossriver.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cross River Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cross River Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cross River Bank
provider_slug: cross-river-bank
slug: cross-river-bank-domain-security
source_filename: cross-river-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crossriver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 04:15:37 2026 GMT\n  hsts: false\n- host: docs.crossriver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 02:59:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crossriver.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cross-river-bank/refs/heads/main/security/cross-river-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Banking as a Service
- Sponsor Bank
- Embedded Finance
- Payments
- ACH
- RTP
- FedNow
- Cards
- Lending
- Stablecoin
---
