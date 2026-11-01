---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jiandanxinli.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: www.jiandanxinli.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Simple Psychology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simple Psychology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Simple Psychology
provider_slug: simple-psychology
slug: simple-psychology-domain-security
source_filename: simple-psychology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jiandanxinli.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: jiandanxinli.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/simple-psychology/security/simple-psychology-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
---
