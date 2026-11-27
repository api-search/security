---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hoodl2.com
  spf: true
hosts:
- cert_expires: Dec 23 18:31:49 2026 GMT
  host: hoodl2.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HoodL2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HoodL2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HoodL2
provider_slug: hoodl2-com
slug: hoodl2-com-domain-security
source_filename: hoodl2-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hoodl2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 18:31:49 2026 GMT\n  hsts: false\ndomains:\n- domain: hoodl2.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hoodl2-com/security/hoodl2-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Blockchain
- Robinhood Chain
- DeFi
- Research
- Cryptocurrency
---
