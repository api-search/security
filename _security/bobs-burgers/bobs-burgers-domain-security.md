---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: herokuapp.com
  spf: false
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: bobs-burgers-api-ui.herokuapp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bobs Burgers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bob''s Burgers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Bob's Burgers
provider_slug: bobs-burgers
slug: bobs-burgers-domain-security
source_filename: bobs-burgers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bobs-burgers-api-ui.herokuapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: herokuapp.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bobs-burgers/refs/heads/main/security/bobs-burgers-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Video
- Public APIs
---
