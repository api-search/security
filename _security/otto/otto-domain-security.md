---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: myotto.net
  spf: false
hosts:
- cert_expires: Sep 17 08:17:10 2026 GMT
  host: myotto.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Otto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OTTO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OTTO
provider_slug: otto
slug: otto-domain-security
source_filename: otto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myotto.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 08:17:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: myotto.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/otto/refs/heads/main/security/otto-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
