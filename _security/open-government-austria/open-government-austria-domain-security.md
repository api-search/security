---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gv.at
  spf: false
hosts:
- cert_expires: Mar  2 13:58:12 2027 GMT
  host: www.data.gv.at
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Austria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Austria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Open Government, Austria
provider_slug: open-government-austria
slug: open-government-austria-domain-security
source_filename: open-government-austria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.data.gv.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 13:58:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gv.at\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-austria/refs/heads/main/security/open-government-austria-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Government
- Public APIs
---
