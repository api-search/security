---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ascend3d.com
  spf: true
hosts:
- cert_expires: Nov 14 14:27:45 2026 GMT
  host: ascend3d.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ascend3Dbe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ascend3dbe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ascend3dbe
provider_slug: ascend3dbe
slug: ascend3dbe-domain-security
source_filename: ascend3dbe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ascend3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 14:27:45 2026 GMT\n  hsts: false\ndomains:\n- domain: ascend3d.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ascend3dbe/refs/heads/main/security/ascend3dbe-domain-security.yml
summary_line: TLSv1.3
tags:
- Robotics
- Automation
- Machine Vision
- Metrology
- Manufacturing
- Software
---
