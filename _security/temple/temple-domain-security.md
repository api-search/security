---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: temple.capital
  spf: true
hosts:
- cert_expires: Aug 11 02:00:16 2026 GMT
  host: www.temple.capital
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Temple Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Temple, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Temple
provider_slug: temple
slug: temple-domain-security
source_filename: temple-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.temple.capital\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 02:00:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: temple.capital\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temple/refs/heads/main/security/temple-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Cryptocurrency
- Digital Assets
- Hedge Fund
- Algorithmic Trading
- Quantitative Trading
- Machine Learning
- Asset Management
- Investment
---
