---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dearovo.com
  spf: true
hosts:
- cert_expires: Jan 23 02:05:24 2027 GMT
  host: dearovo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dearovo Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dearovo-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: dearovo-com
provider_slug: dearovo-com
slug: dearovo-com-domain-security
source_filename: dearovo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dearovo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 02:05:24 2027 GMT\n  hsts: false\ndomains:\n- domain: dearovo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dearovo-com/security/dearovo-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Romance
- Relationship
---
