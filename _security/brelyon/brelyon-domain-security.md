---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brelyon.com
  spf: true
hosts:
- cert_expires: Sep  6 11:52:55 2026 GMT
  host: www.brelyon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brelyon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brelyon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brelyon
provider_slug: brelyon
slug: brelyon-domain-security
source_filename: brelyon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brelyon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 11:52:55 2026 GMT\n  hsts: false\ndomains:\n- domain: brelyon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brelyon/refs/heads/main/security/brelyon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Displays
- Hardware
- Immersive Technology
- Virtual Reality
- Simulation and Training
- Automotive HMI
- Optics
- Visualization
---
