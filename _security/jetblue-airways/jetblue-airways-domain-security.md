---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jetblue.com
  spf: true
hosts:
- cert_expires: Sep 26 02:43:03 2026 GMT
  host: www.jetblue.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jetblue Airways Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JetBlue Airways, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: JetBlue Airways
provider_slug: jetblue-airways
slug: jetblue-airways-domain-security
source_filename: jetblue-airways-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jetblue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 02:43:03 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: jetblue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetblue-airways/refs/heads/main/security/jetblue-airways-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Airlines
- Aviation
- Fortune 500
- Travel
---
