---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prodigyfinance.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: prodigyfinance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prodigy Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prodigy Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Prodigy Finance
provider_slug: prodigy-finance
slug: prodigy-finance-domain-security
source_filename: prodigy-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prodigyfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: prodigyfinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prodigy-finance/refs/heads/main/security/prodigy-finance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Education
- Lending
- Student Loans
- Financial Services
- Consumer Finance
---
