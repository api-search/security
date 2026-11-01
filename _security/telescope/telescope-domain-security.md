---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gotelescope.ai
  spf: true
hosts:
- host: www.gotelescope.ai
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Telescope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telescope, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Telescope
provider_slug: telescope
slug: telescope-domain-security
source_filename: telescope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gotelescope.ai\n  https: false\ndomains:\n- domain: gotelescope.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/telescope/security/telescope-domain-security.yml
summary_line: DMARC
tags:
- Company
- Telescope
- API
- Data
- Analytics
- Platform
---
