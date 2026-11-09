---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cabinetproject.app
  spf: true
hosts:
- cert_expires: Dec 30 07:31:50 2026 GMT
  host: cabinetproject.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cabinetproject App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Design Master Solutions LLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Design Master Solutions LLC
provider_slug: cabinetproject-app
slug: cabinetproject-app-domain-security
source_filename: cabinetproject-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cabinetproject.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 07:31:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cabinetproject.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cabinetproject-app/security/cabinetproject-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cabinet Software
- Quoting
- Dealer Tools
- QuickBooks Integration
---
