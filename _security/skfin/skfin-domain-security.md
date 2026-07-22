---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: skfin.in
  spf: true
hosts:
- cert_expires: Oct 23 07:06:36 2026 GMT
  host: skfin.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Skfin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SK Finance Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SK Finance Ltd
provider_slug: skfin
slug: skfin-domain-security
source_filename: skfin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skfin.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 07:06:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: skfin.in\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skfin/refs/heads/main/security/skfin-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Lending
- NBFC
- Vehicle Finance
- Small Business Loans
- India
- Fintech
---
