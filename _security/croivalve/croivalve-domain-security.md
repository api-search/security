---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: croivalve.com
  spf: true
hosts:
- cert_expires: Jan 30 22:25:27 2027 GMT
  host: www.croivalve.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CroíValve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CroíValve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CroíValve
provider_slug: croivalve
slug: croivalve-domain-security
source_filename: croivalve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.croivalve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 22:25:27 2027 GMT\n  hsts: false\ndomains:\n- domain: croivalve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/croivalve/security/croivalve-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Medical Devices
- Heart Valve
- Tricuspid Regurgitation
- Structural Heart
- Cardiovascular
- Clinical Stage
- Dublin
- Ireland
---
