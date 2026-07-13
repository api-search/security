---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: px4.io
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: docs.px4.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dronecode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dronecode Foundation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dronecode Foundation
provider_slug: dronecode
slug: dronecode-domain-security
source_filename: dronecode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.px4.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: px4.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dronecode/refs/heads/main/security/dronecode-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Drones
- Linux Foundation
- Robotics
- UAV
---
