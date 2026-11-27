---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: atomandbits.com
  spf: true
hosts:
- cert_expires: Jan 24 21:30:39 2027 GMT
  host: atomandbits.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: atomandbits-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for atomandbits-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: atomandbits-com
provider_slug: atomandbits-com
slug: atomandbits-com-domain-security
source_filename: atomandbits-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atomandbits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 21:30:39 2027 GMT\n  hsts: false\ndomains:\n- domain: atomandbits.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/atomandbits-com/security/atomandbits-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
