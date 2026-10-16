---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spinitron.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: spinitron.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spinitron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spinitron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spinitron
provider_slug: spinitron
slug: spinitron-domain-security
source_filename: spinitron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spinitron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: spinitron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spinitron/refs/heads/main/security/spinitron-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music
- Radio
- Playlist
- Community
- Broadcasting
---
