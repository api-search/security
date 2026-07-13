---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tripo3d.ai
  spf: true
hosts:
- cert_expires: Aug 26 06:01:55 2026 GMT
  host: www.tripo3d.ai
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:02:23 2026 GMT
  host: platform.tripo3d.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: api.tripo3d.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tripo3D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tripo3D, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tripo3D
provider_slug: tripo3d
slug: tripo3d-domain-security
source_filename: tripo3d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tripo3d.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:01:55 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\n- host: platform.tripo3d.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:02:23 2026 GMT\n  hsts: false\n- host: api.tripo3d.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tripo3d.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripo3d/refs/heads/main/security/tripo3d-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- 3D
- Generation
- API
- Mesh
- Texturing
---
