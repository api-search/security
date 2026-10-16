---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: peltarion.com
  spf: true
hosts:
- host: peltarion.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Peltarion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peltarion, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Peltarion
provider_slug: peltarion
slug: peltarion-domain-security
source_filename: peltarion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: peltarion.com\n  https: false\ndomains:\n- domain: peltarion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peltarion/refs/heads/main/security/peltarion-domain-security.yml
summary_line: DMARC
tags:
- Company
- AI
- Platform
- Machine-Learning
- Deep-Learning
---
