---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: videofied.com
  spf: true
hosts:
- host: www.videofied.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rsi Video Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RSI Video Technologies, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RSI Video Technologies
provider_slug: rsi-video-technologies
slug: rsi-video-technologies-domain-security
source_filename: rsi-video-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.videofied.com\n  https: false\ndomains:\n- domain: videofied.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rsi-video-technologies/refs/heads/main/security/rsi-video-technologies-domain-security.yml
summary_line: DMARC
tags:
- Company
- Security
- Intrusion Detection
- Video Verification
- Alarm Monitoring
- Central Station Monitoring
- Hardware
- Acquired
---
