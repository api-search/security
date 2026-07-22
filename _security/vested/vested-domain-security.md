---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vestedfinance.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: vestedfinance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vested Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vested, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vested
provider_slug: vested
slug: vested-domain-security
source_filename: vested-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vestedfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: vestedfinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vested/refs/heads/main/security/vested-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- FinTech
- Investing
- Stocks
- ETFs
- Wealth Management
- Brokerage
- India
- US Markets
---
