---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lifttrackapp.com
  spf: true
hosts:
- cert_expires: Jan 23 23:05:50 2027 GMT
  host: lifttrackapp.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LiftTrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiftTrack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LiftTrack
provider_slug: lifttrackapp-com
slug: lifttrackapp-com-domain-security
source_filename: lifttrackapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lifttrackapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:05:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: lifttrackapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lifttrackapp-com/security/lifttrackapp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Strength Training
- GarminIntegration
- Artificial Intelligence
- Health Tech
---
