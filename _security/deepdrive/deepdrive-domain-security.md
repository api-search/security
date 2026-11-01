---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: deepdrive.io
  spf: true
hosts:
- cert_expires: Jan  4 02:17:42 2027 GMT
  host: deepdrive.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deepdrive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deepdrive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Deepdrive
provider_slug: deepdrive
slug: deepdrive-domain-security
source_filename: deepdrive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepdrive.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 02:17:42 2027 GMT\n  hsts: false\ndomains:\n- domain: deepdrive.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/deepdrive/security/deepdrive-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Technology
- Automotive
- Artificial Intelligence
- Data
---
