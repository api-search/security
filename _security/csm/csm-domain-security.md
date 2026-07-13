---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:eng@csm.ai"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: csm.ai
  spf: true
hosts:
- host: www.csm.ai
  https: false
- host: docs.csm.ai
  https: false
- host: api.csm.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Csm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Common Sense Machines, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Common Sense Machines
provider_slug: csm
slug: csm-domain-security
source_filename: csm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.csm.ai\n  https: false\n- host: docs.csm.ai\n  https: false\n- host: api.csm.ai\n  https: false\ndomains:\n- domain: csm.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:eng@csm.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/csm/refs/heads/main/security/csm-domain-security.yml
summary_line: DMARC
tags:
- AI
- 3D
- World Models
- Scene Generation
- Generative
- Robotics
---
