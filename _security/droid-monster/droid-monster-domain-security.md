---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: droid.monster
  spf: true
hosts:
- cert_expires: Feb  1 14:47:13 2027 GMT
  host: droid.monster
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Droid Monster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Droid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Droid
provider_slug: droid-monster
slug: droid-monster-domain-security
source_filename: droid-monster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: droid.monster\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 14:47:13 2027 GMT\n  hsts: false\ndomains:\n- domain: droid.monster\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/droid-monster/security/droid-monster-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Robotics
- Data
- Reference
- Open Data
---
