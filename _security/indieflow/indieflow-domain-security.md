---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: indieflow.me
  spf: false
hosts:
- host: indieflow.me
  https: false
kind: domain-security
layout: security
method: probed
name: Indieflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IndieFlow, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: IndieFlow
provider_slug: indieflow
slug: indieflow-domain-security
source_filename: indieflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indieflow.me\n  https: false\ndomains:\n- domain: indieflow.me\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indieflow/refs/heads/main/security/indieflow-domain-security.yml
summary_line: DMARC
tags:
- Company
- Music
- Music Distribution
- Independent Artists
- Royalties
- Music Management
- Streaming
- Artist Tools
- Techstars
---
