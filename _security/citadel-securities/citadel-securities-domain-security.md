---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: citadelsecurities.com
  spf: true
hosts:
- cert_expires: Oct  3 03:26:22 2026 GMT
  host: www.citadelsecurities.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Citadel Securities Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citadel Securities, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Citadel Securities
provider_slug: citadel-securities
slug: citadel-securities-domain-security
source_filename: citadel-securities-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.citadelsecurities.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:26:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: citadelsecurities.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citadel-securities/refs/heads/main/security/citadel-securities-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Financial Services
- Market Maker
- Electronic Trading
- Liquidity
- Capital Markets
---
