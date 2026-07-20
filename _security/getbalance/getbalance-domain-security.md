---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getbalance.com
  spf: true
hosts:
- cert_expires: Sep  6 18:37:34 2026 GMT
  host: www.getbalance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: dashboard.getbalance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: api.getbalance.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Getbalance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Getbalance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Getbalance
provider_slug: getbalance
slug: getbalance-domain-security
source_filename: getbalance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getbalance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:37:34 2026 GMT\n  hsts: false\n- host: dashboard.getbalance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.getbalance.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: getbalance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getbalance/refs/heads/main/security/getbalance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- B2B Payments
- Trade Credit
- BNPL
- Accounts Receivable
- Financial Infrastructure
- Fintech
- Order-to-Cash
- Embedded Finance
- Marketplace
---
