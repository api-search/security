---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: autodesk.com
  spf: true
hosts:
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: www.autodesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autodesk Powermill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autodesk PowerMill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Autodesk PowerMill
provider_slug: autodesk-powermill
slug: autodesk-powermill-domain-security
source_filename: autodesk-powermill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: autodesk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk-powermill/refs/heads/main/security/autodesk-powermill-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- 5-Axis Machining
- CAM
- CNC
- Machining
- Manufacturing
- Aerospace
- Automotive
- Toolpath Generation
---
