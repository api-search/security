---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: novacredit.com
  spf: true
hosts:
- cert_expires: Nov 16 23:59:59 2026 GMT
  host: novacredit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nova Credit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nova Credit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nova Credit
provider_slug: nova-credit
slug: nova-credit-domain-security
source_filename: nova-credit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novacredit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: novacredit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nova-credit/refs/heads/main/security/nova-credit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Credit Data
- Consumer Credit
- Credit Bureau
- Income Verification
- Underwriting
- Fintech
- Financial Services
- Lending
- Cash Flow Underwriting
- Identity
---
