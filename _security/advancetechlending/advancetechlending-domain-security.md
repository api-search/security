---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: advance.ph
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: advance.ph
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Advancetechlending Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advance Tech Lending, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Advance Tech Lending
provider_slug: advancetechlending
slug: advancetechlending-domain-security
source_filename: advancetechlending-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: advance.ph\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: advance.ph\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advancetechlending/refs/heads/main/security/advancetechlending-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Financial Services
- Fintech
- Lending
- Salary Advance
- Earned Wage Access
- Invoice Financing
- Payroll
- Employee Benefits
- Philippines
- Southeast Asia
- Company
---
