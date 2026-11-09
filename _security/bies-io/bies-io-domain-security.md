---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bies.io
  spf: false
hosts:
- cert_expires: Dec 31 01:11:48 2026 GMT
  host: bies.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bies Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BIES Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: BIES Studio
provider_slug: bies-io
slug: bies-io-domain-security
source_filename: bies-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bies.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 01:11:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bies.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bies-io/security/bies-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Software
- Productivity
- 3D
- Collaboration
- Innovation
---
