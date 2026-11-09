---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: adson.jp
  spf: true
hosts:
- cert_expires: Dec 31 16:56:57 2026 GMT
  host: adson.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adson Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADSON, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ADSON
provider_slug: adson-jp
slug: adson-jp-domain-security
source_filename: adson-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adson.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 16:56:57 2026 GMT\n  hsts: false\ndomains:\n- domain: adson.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/adson-jp/security/adson-jp-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Design
- Development
- Media
- Data
- Artificial Intelligence
---
