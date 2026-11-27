---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nara-tour.com
  spf: false
hosts:
- cert_expires: May 25 15:53:08 2027 GMT
  host: nara-tour.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: nara-tour-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nara-tour-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: nara-tour-com
provider_slug: nara-tour-com
slug: nara-tour-com-domain-security
source_filename: nara-tour-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nara-tour.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 25 15:53:08 2027 GMT\n  hsts: null\ndomains:\n- domain: nara-tour.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nara-tour-com/security/nara-tour-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
