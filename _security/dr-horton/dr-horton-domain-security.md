---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: drhorton.com
  spf: true
hosts:
- cert_expires: Aug 15 23:44:31 2026 GMT
  host: www.drhorton.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dr Horton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for D.R. Horton, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: D.R. Horton
provider_slug: dr-horton
slug: dr-horton-domain-security
source_filename: dr-horton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drhorton.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 15 23:44:31 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: drhorton.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dr-horton/refs/heads/main/security/dr-horton-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Fortune 500
- Homebuilder
- Real Estate
- Construction
---
