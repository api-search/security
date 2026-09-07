---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: acornfinance.com
  spf: true
hosts:
- cert_expires: Oct 24 23:08:22 2026 GMT
  host: www.acornfinance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: docs.acornfinance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: api.acornfinance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Acorn Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acorn Finance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Acorn Finance
provider_slug: acorn-finance
slug: acorn-finance-domain-security
source_filename: acorn-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acornfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:08:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.acornfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.acornfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: acornfinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acorn-finance/refs/heads/main/security/acorn-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Lending
- Loans
- Home Improvement
- Embedded Finance
- Point of Sale
- Consumer Finance
- Fintech
- Webhooks
---
