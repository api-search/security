---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vidcaster.com
  spf: true
hosts:
- host: vidcaster.com
  https: false
kind: domain-security
layout: security
method: probed
name: Vidcaster Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vidcaster, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vidcaster
provider_slug: vidcaster
slug: vidcaster-domain-security
source_filename: vidcaster-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vidcaster.com\n  https: false\ndomains:\n- domain: vidcaster.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidcaster/refs/heads/main/security/vidcaster-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Video
- Video Platform
- Video Marketing
- Video Hosting
- Video SEO
- Defunct
---
