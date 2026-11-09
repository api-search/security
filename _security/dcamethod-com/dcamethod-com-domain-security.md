---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dcamethod.com
  spf: false
hosts:
- cert_expires: Dec 16 10:44:20 2026 GMT
  host: dcamethod.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dcamethod Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DCA Method, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DCA Method
provider_slug: dcamethod-com
slug: dcamethod-com-domain-security
source_filename: dcamethod-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dcamethod.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 10:44:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dcamethod.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dcamethod-com/security/dcamethod-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Investment
- Calculator
- Cryptocurrency
- Education
---
