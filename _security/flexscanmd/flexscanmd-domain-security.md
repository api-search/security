---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flexscanmd.com
  spf: true
hosts:
- cert_expires: Jan 18 00:46:31 2027 GMT
  host: flexscanmd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FlexScanMD Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlexScanMD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FlexScanMD
provider_slug: flexscanmd
slug: flexscanmd-domain-security
source_filename: flexscanmd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flexscanmd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 00:46:31 2027 GMT\n  hsts: false\ndomains:\n- domain: flexscanmd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/flexscanmd/security/flexscanmd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Inventory
- Medical Software
- Cloud‑based
- Compliance
---
