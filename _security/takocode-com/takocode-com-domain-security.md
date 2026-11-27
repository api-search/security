---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: takocode.com
  spf: true
hosts:
- cert_expires: Jan  9 06:31:53 2027 GMT
  host: takocode.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TakoCode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TakoCode, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TakoCode
provider_slug: takocode-com
slug: takocode-com-domain-security
source_filename: takocode-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: takocode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 06:31:53 2027 GMT\n  hsts: false\ndomains:\n- domain: takocode.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/takocode-com/security/takocode-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Low-code
- App Builder
- SaaS
- Company
---
