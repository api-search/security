---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: regular.eu
  spf: true
hosts:
- cert_expires: Sep  2 02:36:23 2026 GMT
  host: regular.eu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regular Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regular Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Regular Finance
provider_slug: regular-finance
slug: regular-finance-domain-security
source_filename: regular-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: regular.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 02:36:23 2026 GMT\n  hsts: false\ndomains:\n- domain: regular.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regular-finance/refs/heads/main/security/regular-finance-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Fintech
- Stablecoins
- Digital Assets
- Yield
- Savings
- Cryptocurrency
- France
---
