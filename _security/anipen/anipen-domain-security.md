---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: anipen.com
  spf: false
hosts:
- host: www.anipen.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anipen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anipen, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Anipen
provider_slug: anipen
slug: anipen-domain-security
source_filename: anipen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anipen.com\n  https: false\ndomains:\n- domain: anipen.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anipen/refs/heads/main/security/anipen-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- XR
- AR
- AI
- Metaverse
---
