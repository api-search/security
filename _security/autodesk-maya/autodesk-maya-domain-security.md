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
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: help.autodesk.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Autodesk Maya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autodesk Maya, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Autodesk Maya
provider_slug: autodesk-maya
slug: autodesk-maya-domain-security
source_filename: autodesk-maya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autodesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: null\n- host: help.autodesk.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: autodesk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autodesk-maya/refs/heads/main/security/autodesk-maya-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- 3D Graphics
- Animation
- Game Development
- Modeling
- Rendering
- Visual Effects
- VFX
- CAD
---
