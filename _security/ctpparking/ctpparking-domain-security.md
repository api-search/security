---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: icnctp.com
  spf: true
hosts:
- host: icnctp.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ctpparking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ctpparking, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ctpparking
provider_slug: ctpparking
slug: ctpparking-domain-security
source_filename: ctpparking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: icnctp.com\n  https: false\ndomains:\n- domain: icnctp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ctpparking/refs/heads/main/security/ctpparking-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Parking
- SmartCity
- IoT
- China
---
