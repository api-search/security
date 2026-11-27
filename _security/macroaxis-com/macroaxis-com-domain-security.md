---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: macroaxis.com
  spf: false
hosts:
- cert_expires: Apr  1 23:59:59 2027 GMT
  host: macroaxis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Macroaxis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Macroaxis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Macroaxis
provider_slug: macroaxis-com
slug: macroaxis-com-domain-security
source_filename: macroaxis-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: macroaxis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: macroaxis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/macroaxis-com/security/macroaxis-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Finance
- Investment
- Portfolio
- Analytics
- Artificial Intelligence
---
