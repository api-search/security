---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tryjeeves.com
  spf: true
hosts:
- cert_expires: Sep 28 19:58:22 2026 GMT
  host: www.tryjeeves.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jeeves Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jeeves, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Jeeves
provider_slug: jeeves
slug: jeeves-domain-security
source_filename: jeeves-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tryjeeves.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:58:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tryjeeves.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jeeves/refs/heads/main/security/jeeves-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Corporate Cards
- Expense Management
- Cross-Border Payments
- Spend Management
- Global Payments
- Stablecoins
- Financial Services
- Corporate Credit
---
