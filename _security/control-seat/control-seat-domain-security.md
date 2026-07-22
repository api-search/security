---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: controlseat.com
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.controlseat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Control Seat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Control Seat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Control Seat
provider_slug: control-seat
slug: control-seat-domain-security
source_filename: control-seat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.controlseat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: controlseat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/control-seat/refs/heads/main/security/control-seat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SCADA
- Industrial
- Monitoring
- Workflow Automation
- Manufacturing
- Analytics
- Real-Time
- IoT
- Historian
---
