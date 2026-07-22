---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jolt.io
  spf: true
hosts:
- host: www.jolt.io
  https: false
kind: domain-security
layout: security
method: probed
name: Jolt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jolt, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: jolt
provider_slug: jolt
slug: jolt-domain-security
source_filename: jolt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jolt.io\n  https: false\ndomains:\n- domain: jolt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jolt/refs/heads/main/security/jolt-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
