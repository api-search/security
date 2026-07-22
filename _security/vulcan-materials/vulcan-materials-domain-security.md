---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vulcan-materials.com
  spf: true
hosts:
- host: www.vulcan-materials.com
  https: false
kind: domain-security
layout: security
method: probed
name: Vulcan Materials Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vulcan Materials Company, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vulcan Materials Company
provider_slug: vulcan-materials
slug: vulcan-materials-domain-security
source_filename: vulcan-materials-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vulcan-materials.com\n  https: false\ndomains:\n- domain: vulcan-materials.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vulcan-materials/refs/heads/main/security/vulcan-materials-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Aggregates
- Construction
- Fortune 500
- Infrastructure
- Materials
- Mining
---
