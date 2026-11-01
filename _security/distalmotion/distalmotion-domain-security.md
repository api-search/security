---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: distalmotion.com
  spf: true
hosts:
- cert_expires: Jan 19 02:56:10 2027 GMT
  host: www.distalmotion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Distalmotion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Distalmotion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Distalmotion
provider_slug: distalmotion
slug: distalmotion-domain-security
source_filename: distalmotion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.distalmotion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 02:56:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: distalmotion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/distalmotion/security/distalmotion-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Robotics
- Medical Devices
- Surgery
- Healthcare
- Switzerland
---
