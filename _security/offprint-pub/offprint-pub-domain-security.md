---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: offprint.pub
  spf: true
hosts:
- cert_expires: Feb  4 14:48:07 2027 GMT
  host: offprint.pub
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Offprint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Offprint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Offprint
provider_slug: offprint-pub
slug: offprint-pub-domain-security
source_filename: offprint-pub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: offprint.pub\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 14:48:07 2027 GMT\n  hsts: false\ndomains:\n- domain: offprint.pub\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/offprint-pub/security/offprint-pub-domain-security.yml
summary_line: TLSv1.3
tags:
- Content Extraction
- PDF Generation
- Markdown
- Artificial Intelligence
- Publishing
---
