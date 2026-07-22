---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brightviewtechnologies.com
  spf: true
hosts:
- cert_expires: Oct  5 23:05:56 2026 GMT
  host: www.brightviewtechnologies.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bright View Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bright View Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bright View Technologies
provider_slug: bright-view-technologies
slug: bright-view-technologies-domain-security
source_filename: bright-view-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightviewtechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:05:56 2026 GMT\n  hsts: false\ndomains:\n- domain: brightviewtechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bright-view-technologies/refs/heads/main/security/bright-view-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Optics
- Photonics
- Micro Lens Array
- Optical Films
- Computational Optics
- LiDAR
- Displays
- LED Lighting
- AR/VR
- Manufacturing
- Hardware
---
