---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gfycat.com
  spf: true
hosts:
- host: developers.gfycat.com
  https: false
kind: domain-security
layout: security
method: probed
name: Gfycat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gfycat, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gfycat
provider_slug: gfycat
slug: gfycat-domain-security
source_filename: gfycat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.gfycat.com\n  https: false\ndomains:\n- domain: gfycat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gfycat/refs/heads/main/security/gfycat-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Photography
- Public APIs
---
