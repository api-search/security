---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: liveaction.com
  spf: true
hosts:
- cert_expires: Aug 30 14:46:09 2026 GMT
  host: liveaction.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liveaction Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiveAction, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LiveAction
provider_slug: liveaction
slug: liveaction-domain-security
source_filename: liveaction-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liveaction.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:46:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: liveaction.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveaction/refs/heads/main/security/liveaction-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Network Monitoring
- Network Observability
- Network Performance Monitoring
- Packet Capture
- Network Forensics
- SD-WAN
- Telemetry
---
