---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: morewis.com
  spf: true
hosts:
- host: morewis.com
  https: false
kind: domain-security
layout: security
method: probed
name: Morewis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for morewis, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: morewis
provider_slug: morewis
slug: morewis-domain-security
source_filename: morewis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: morewis.com\n  https: false\ndomains:\n- domain: morewis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morewis/refs/heads/main/security/morewis-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Manufacturing
- MES
- MOM
- Industrial IoT
- Low-Code
- Industrial AI
- Smart Manufacturing
- China
---
