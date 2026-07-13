---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: amethyste.moe
  spf: true
hosts:
- host: api.amethyste.moe
  https: false
kind: domain-security
layout: security
method: probed
name: Am Thyste Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Améthyste, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Améthyste
provider_slug: am-thyste
slug: am-thyste-domain-security
source_filename: am-thyste-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.amethyste.moe\n  https: false\ndomains:\n- domain: amethyste.moe\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/am-thyste/refs/heads/main/security/am-thyste-domain-security.yml
summary_line: DNSSEC
tags:
- Art And Design
- Public APIs
---
