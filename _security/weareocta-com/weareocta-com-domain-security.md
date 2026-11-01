---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: weareocta.com
  spf: true
hosts:
- cert_expires: Jan  7 00:13:27 2027 GMT
  host: weareocta.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Weareocta Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Octa
provider_slug: weareocta-com
slug: weareocta-com-domain-security
source_filename: weareocta-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weareocta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 00:13:27 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: weareocta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/weareocta-com/security/weareocta-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Accounting
- SaaS
- Workforce
---
