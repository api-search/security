---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jbpscapital.com
  spf: true
hosts:
- cert_expires: Feb  8 15:33:05 2027 GMT
  host: jbpscapital.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JBPS Capital LLC Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JBPS Capital LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JBPS Capital LLC
provider_slug: jbpscapital-com
slug: jbpscapital-com-domain-security
source_filename: jbpscapital-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jbpscapital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 15:33:05 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jbpscapital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jbpscapital-com/security/jbpscapital-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Research
- Technology
- Systematic
- MarketModels
---
