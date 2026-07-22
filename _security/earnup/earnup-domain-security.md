---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: earnup.com
  spf: true
hosts:
- cert_expires: Sep 16 17:07:23 2026 GMT
  host: www.earnup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Earnup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EarnUp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EarnUp
provider_slug: earnup
slug: earnup-domain-security
source_filename: earnup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.earnup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 17:07:23 2026 GMT\n  hsts: false\ndomains:\n- domain: earnup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earnup/refs/heads/main/security/earnup-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Financial Services
- Debt Repayment
- Personal Finance
- Payments
- Financial Wellness
- Lending
---
