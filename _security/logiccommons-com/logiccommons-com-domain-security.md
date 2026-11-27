---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: logiccommons.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: logiccommons.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LogicCommons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LogicCommons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LogicCommons
provider_slug: logiccommons-com
slug: logiccommons-com-domain-security
source_filename: logiccommons-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: logiccommons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: logiccommons.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/logiccommons-com/security/logiccommons-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Calculator
- Engineering
- Finance
- Personal
- Open Data
---
