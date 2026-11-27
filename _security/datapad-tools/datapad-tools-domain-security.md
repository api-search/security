---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: datapad.tools
  spf: false
hosts:
- cert_expires: Dec 31 04:36:18 2026 GMT
  host: datapad.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Data Pad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data Pad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Data Pad
provider_slug: datapad-tools
slug: datapad-tools-domain-security
source_filename: datapad-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datapad.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 04:36:18 2026 GMT\n  hsts: false\ndomains:\n- domain: datapad.tools\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/datapad-tools/security/datapad-tools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Tools
- Healthcare
- Business
- Open Source
- Free
---
