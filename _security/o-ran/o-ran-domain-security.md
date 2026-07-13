---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: o-ran.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: o-ran-sc.org
  spf: false
hosts:
- cert_expires: Aug 16 18:31:40 2026 GMT
  host: o-ran.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 13:37:31 2026 GMT
  host: docs.o-ran-sc.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: O Ran Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for O-RAN, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: O-RAN
provider_slug: o-ran
slug: o-ran-domain-security
source_filename: o-ran-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: o-ran.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:31:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.o-ran-sc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:37:31 2026 GMT\n  hsts: false\ndomains:\n- domain: o-ran.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: o-ran-sc.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/o-ran/refs/heads/main/security/o-ran-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Linux Foundation
- Mobile Network
- Open Source
- RAN
- Radio
- Telecom
---
