---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: metrist.io
  spf: true
hosts:
- host: www.metrist.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Metrist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metrist, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Metrist
provider_slug: metrist
slug: metrist-domain-security
source_filename: metrist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.metrist.io\n  https: false\ndomains:\n- domain: metrist.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/metrist/security/metrist-domain-security.yml
summary_line: DMARC
tags:
- Monitoring
- Observability
- DevOps
- Cloud
- API
---
