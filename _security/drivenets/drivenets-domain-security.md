---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: drivenets.com
  spf: true
hosts:
- cert_expires: Aug 27 23:59:59 2026 GMT
  host: www.drivenets.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drivenets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DriveNets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DriveNets
provider_slug: drivenets
slug: drivenets-domain-security
source_filename: drivenets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drivenets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: drivenets.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drivenets/refs/heads/main/security/drivenets-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Ai Ml
- Networking
- Network Operating System
- Network Automation
- Disaggregated Networking
- Cloud Networking
- AI Fabric
- Telco
- NETCONF
---
