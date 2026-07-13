---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: true
  domain: shikimori.one
  spf: false
hosts:
- host: shikimori.one
  https: false
kind: domain-security
layout: security
method: probed
name: Shikimori Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shikimori, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Shikimori
provider_slug: shikimori
slug: shikimori-domain-security
source_filename: shikimori-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shikimori.one\n  https: false\ndomains:\n- domain: shikimori.one\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shikimori/refs/heads/main/security/shikimori-domain-security.yml
summary_line: DNSSEC
tags:
- Anime
- Public APIs
---
