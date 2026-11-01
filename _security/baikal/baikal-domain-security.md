---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sabre.io
  spf: true
hosts:
- cert_expires: Jan 21 10:58:21 2027 GMT
  host: sabre.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Baikal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baikal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Baikal
provider_slug: baikal
slug: baikal-domain-security
source_filename: baikal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sabre.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 10:58:21 2027 GMT\n  hsts: false\ndomains:\n- domain: sabre.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/baikal/security/baikal-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- API
- OpenSource
- Calendar
- CardDAV
---
