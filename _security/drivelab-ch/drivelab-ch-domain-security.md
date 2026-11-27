---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: drivelab.ch
  spf: true
hosts:
- cert_expires: Jan  1 01:13:25 2027 GMT
  host: drivelab.ch
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DriveLab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DriveLab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DriveLab
provider_slug: drivelab-ch
slug: drivelab-ch-domain-security
source_filename: drivelab-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drivelab.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 01:13:25 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: drivelab.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/drivelab-ch/security/drivelab-ch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Swiss
- First‑Aid Course
---
