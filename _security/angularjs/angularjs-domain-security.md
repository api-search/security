---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: angularjs.org
  spf: true
hosts:
- cert_expires: Aug 30 23:44:48 2026 GMT
  host: angularjs.org
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 11:43:49 2026 GMT
  host: docs.angularjs.org
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 23:12:25 2026 GMT
  host: code.angularjs.org
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Angularjs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AngularJS, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: AngularJS
provider_slug: angularjs
slug: angularjs-domain-security
source_filename: angularjs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: angularjs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:44:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: docs.angularjs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 11:43:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: code.angularjs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 23:12:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: angularjs.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angularjs/refs/heads/main/security/angularjs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- End Of Life
- Framework
- Frontend
- Google
- JavaScript
- Legacy
- MVC
- Open Source
- Single Page Application
---
