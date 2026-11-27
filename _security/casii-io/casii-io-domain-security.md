---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: casii.io
  spf: true
hosts:
- cert_expires: Jan 17 00:18:07 2027 GMT
  host: casii.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Casii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Casii, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Casii
provider_slug: casii-io
slug: casii-io-domain-security
source_filename: casii-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: casii.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 00:18:07 2027 GMT\n  hsts: false\ndomains:\n- domain: casii.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/casii-io/security/casii-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Sales
- Lead Management
- Multilingual
- Outreach
- Prospecting
---
