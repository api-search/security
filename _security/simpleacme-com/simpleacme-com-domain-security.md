---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: simpleacme.com
  spf: false
hosts:
- cert_expires: Feb  5 18:49:32 2027 GMT
  host: simpleacme.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SimpleACME Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimpleACME, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SimpleACME
provider_slug: simpleacme-com
slug: simpleacme-com-domain-security
source_filename: simpleacme-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simpleacme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 18:49:32 2027 GMT\n  hsts: false\ndomains:\n- domain: simpleacme.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/simpleacme-com/security/simpleacme-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Certificates
- DNS‑01
- Wildcard
- ACME
- Integration
---
