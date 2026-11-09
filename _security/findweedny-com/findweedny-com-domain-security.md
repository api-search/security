---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: findweedny.com
  spf: true
hosts:
- cert_expires: Feb  4 01:54:44 2027 GMT
  host: findweedny.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Findweedny Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FindWeedNY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: FindWeedNY
provider_slug: findweedny-com
slug: findweedny-com-domain-security
source_filename: findweedny-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: findweedny.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 01:54:44 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: findweedny.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/findweedny-com/security/findweedny-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cannabis
- NewYork
- Directory
- OpenData
- Maps
---
