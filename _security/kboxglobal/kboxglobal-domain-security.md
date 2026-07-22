---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kboxglobal.com
  spf: false
hosts:
- cert_expires: Sep  8 10:35:27 2026 GMT
  host: www.kboxglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kboxglobal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kboxglobal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: kboxglobal
provider_slug: kboxglobal
slug: kboxglobal-domain-security
source_filename: kboxglobal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kboxglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 10:35:27 2026 GMT\n  hsts: null\ndomains:\n- domain: kboxglobal.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kboxglobal/refs/heads/main/security/kboxglobal-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
