---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:root@blender.org"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: blender.org
  spf: true
hosts:
- cert_expires: Sep 20 04:33:43 2026 GMT
  host: www.blender.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 08:46:52 2026 GMT
  host: docs.blender.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 16:01:16 2026 GMT
  host: extensions.blender.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blender Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blender, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Blender
provider_slug: blender
slug: blender-domain-security
source_filename: blender-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blender.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 04:33:43 2026 GMT\n  hsts: false\n- host: docs.blender.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:46:52 2026 GMT\n  hsts: false\n- host: extensions.blender.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 16:01:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blender.org\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:root@blender.org\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blender/refs/heads/main/security/blender-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- 3D
- Animation
- Game Development
- Modeling
- Open Source
- Python
- Rendering
- VFX
---
