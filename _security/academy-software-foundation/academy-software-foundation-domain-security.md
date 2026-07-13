---
api_specs:
- filename: academy-software-foundation-opencue.yaml
  format: yaml
  label: OpenCue
  slug: opencue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/openapi/academy-software-foundation-opencue.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aswf.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: openexr.com
  spf: false
hosts:
- cert_expires: Sep  6 18:54:28 2026 GMT
  host: www.aswf.io
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 20:19:25 2026 GMT
  host: openexr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 16:04:23 2026 GMT
  host: www.openvdb.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Academy Software Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Academy Software Foundation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Academy Software Foundation
provider_slug: academy-software-foundation
slug: academy-software-foundation-domain-security
source_filename: academy-software-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aswf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:54:28 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: openexr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:19:25 2026 GMT\n  hsts: false\n- host: www.openvdb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:04:23 2026 GMT\n  hsts: false\ndomains:\n- domain: aswf.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openexr.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/security/academy-software-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Animation
- Color Management
- Film
- Linux Foundation
- Open Source
- Rendering
- Standards
- Visual Effects
- VFX
---
