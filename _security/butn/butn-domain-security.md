---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: butn.co
  spf: true
hosts:
- cert_expires: Oct 15 03:41:10 2026 GMT
  host: www.butn.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Butn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Butn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Butn
provider_slug: butn
slug: butn-domain-security
source_filename: butn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.butn.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 03:41:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: butn.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butn/refs/heads/main/security/butn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Embedded Finance
- Invoice Finance
- Accounts Receivable
- Accounts Payable
- B2B BNPL
- Business Lending
- Cashflow
- Working Capital
---
