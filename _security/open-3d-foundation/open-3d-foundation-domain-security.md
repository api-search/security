---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: o3de.org
  spf: true
hosts:
- cert_expires: Sep 20 19:54:50 2026 GMT
  host: www.o3de.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open 3D Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open 3D Foundation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open 3D Foundation
provider_slug: open-3d-foundation
slug: open-3d-foundation-domain-security
source_filename: open-3d-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.o3de.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:54:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: o3de.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-3d-foundation/refs/heads/main/security/open-3d-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- 3D Engine
- Gaming
- Linux Foundation
- Simulation
---
