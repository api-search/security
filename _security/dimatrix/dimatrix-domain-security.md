---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: diamatrix.com
  spf: true
hosts:
- cert_expires: Dec  9 02:42:44 2026 GMT
  host: diamatrix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dimatrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dimatrix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dimatrix
provider_slug: dimatrix
slug: dimatrix-domain-security
source_filename: dimatrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diamatrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 02:42:44 2026 GMT\n  hsts: false\ndomains:\n- domain: diamatrix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dimatrix/security/dimatrix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Medical
- Ophthalmology
- Surgical Instruments
- Healthcare
- Devices
---
