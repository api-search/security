---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: possiblefinance.com
  spf: true
hosts:
- cert_expires: Oct 12 03:53:53 2026 GMT
  host: www.possiblefinance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Possible Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Possible Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Possible Finance
provider_slug: possible-finance
slug: possible-finance-domain-security
source_filename: possible-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.possiblefinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:53:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: possiblefinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/possible-finance/refs/heads/main/security/possible-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Consumer Lending
- Credit Building
- Personal Finance
- Mobile App
- Financial Services
- Public Benefit Corporation
---
