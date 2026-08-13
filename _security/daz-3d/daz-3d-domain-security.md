---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: daz3d.com
  spf: true
hosts:
- cert_expires: Oct 26 23:14:06 2026 GMT
  host: www.daz3d.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Daz 3D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DAZ 3D, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DAZ 3D
provider_slug: daz-3d
slug: daz-3d-domain-security
source_filename: daz-3d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.daz3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:14:06 2026 GMT\n  hsts: false\ndomains:\n- domain: daz3d.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daz-3d/refs/heads/main/security/daz-3d-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- 3D
- 3D Content
- Digital Assets
- Graphics
- Rendering
- Avatars
- Game Development
- AI Training Data
- Marketplace
- SDK
- Desktop Software
- Creator Tools
---
