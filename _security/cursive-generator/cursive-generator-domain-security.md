---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cursive-generator.app
  spf: true
hosts:
- cert_expires: Dec 10 17:44:42 2026 GMT
  host: cursive-generator.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cursive Generator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cursive Generator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cursive Generator
provider_slug: cursive-generator
slug: cursive-generator-domain-security
source_filename: cursive-generator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cursive-generator.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 17:44:42 2026 GMT\n  hsts: false\ndomains:\n- domain: cursive-generator.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cursive-generator/security/cursive-generator-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Design
- Text
- Font
---
