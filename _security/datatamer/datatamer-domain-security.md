---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: datatamer.com
  spf: true
hosts:
- cert_expires: Jan  3 03:33:58 2027 GMT
  host: datatamer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datatamer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datatamer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Datatamer
provider_slug: datatamer
slug: datatamer-domain-security
source_filename: datatamer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datatamer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 03:33:58 2027 GMT\n  hsts: false\ndomains:\n- domain: datatamer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/datatamer/security/datatamer-domain-security.yml
summary_line: TLSv1.3
tags:
- IT Consulting
- Network Design
- System Analysis
- Software Training
- Computer Repair
- Remote Support
---
