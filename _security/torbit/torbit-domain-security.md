---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: torbit.com
  spf: true
hosts:
- host: torbit.com
  https: false
kind: domain-security
layout: security
method: probed
name: Torbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Torbit, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Torbit
provider_slug: torbit
slug: torbit-domain-security
source_filename: torbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: torbit.com\n  https: false\ndomains:\n- domain: torbit.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/torbit/refs/heads/main/security/torbit-domain-security.yml
summary_line: DMARC
tags:
- Company
- Web Performance
- Real User Monitoring
- Front-End Optimization
- Acquired
- Defunct
---
