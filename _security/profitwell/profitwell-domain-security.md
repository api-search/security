---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paddle.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: profitwell.com
  spf: true
hosts:
- cert_expires: Sep 11 12:23:57 2026 GMT
  host: www.paddle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 06:22:57 2026 GMT
  host: api.profitwell.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Profitwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProfitWell, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ProfitWell
provider_slug: profitwell
slug: profitwell-domain-security
source_filename: profitwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paddle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:23:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.profitwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:22:57 2026 GMT\n  hsts: null\ndomains:\n- domain: paddle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: profitwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/profitwell/refs/heads/main/security/profitwell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Subscription Analytics
- SaaS Metrics
- Revenue Analytics
- Churn
- MRR
- Billing
---
