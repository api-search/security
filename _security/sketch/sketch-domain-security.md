---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sketch.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sketch.cloud
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.sketch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 16:13:42 2026 GMT
  host: developer.sketch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.sketch.cloud
  https: false
kind: domain-security
layout: security
method: probed
name: Sketch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sketch, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sketch
provider_slug: sketch
slug: sketch-domain-security
source_filename: sketch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sketch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.sketch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:13:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sketch.cloud\n  https: false\ndomains:\n- domain: sketch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: sketch.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sketch/refs/heads/main/security/sketch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design
- Collaboration
- Prototyping
- Workspaces
- Documents
- Libraries
- Components
---
