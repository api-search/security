---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lfedge.org
  spf: true
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: lfedge.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lf Edge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LF Edge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LF Edge
provider_slug: lf-edge
slug: lf-edge-domain-security
source_filename: lf-edge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lfedge.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: lfedge.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lf-edge/refs/heads/main/security/lf-edge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Edge Computing
- IoT
- Linux Foundation
- Open Source
---
