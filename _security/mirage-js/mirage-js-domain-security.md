---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: miragejs.com
  spf: false
hosts:
- cert_expires: Sep 14 07:21:31 2026 GMT
  host: miragejs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mirage Js Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mirage JS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mirage JS
provider_slug: mirage-js
slug: mirage-js-domain-security
source_filename: mirage-js-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: miragejs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:21:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: miragejs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mirage-js/refs/heads/main/security/mirage-js-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Mocking
- Testing
- JavaScript
- Open Source
---
