---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: vake.ai
  spf: true
hosts:
- cert_expires: Sep 26 03:36:45 2026 GMT
  host: vake.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vake, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Vake
provider_slug: vake
slug: vake-domain-security
source_filename: vake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vake.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:36:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vake.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vake/refs/heads/main/security/vake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Maritime
- Maritime Domain Awareness
- Satellite Imagery
- Vessel Tracking
- AIS
- Geospatial
- Machine Learning
- Dark Vessels
- Defense
- Situational Awareness
---
