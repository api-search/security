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
- host: csm.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Common Sense Machines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Common Sense Machines, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Common Sense Machines
provider_slug: common-sense-machines
slug: common-sense-machines-domain-security
source_filename: common-sense-machines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: csm.ai\n  https: false\ndomains:\n- domain: csm.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:eng@csm.ai\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/common-sense-machines/refs/heads/main/security/common-sense-machines-domain-security.yml
summary_line: DMARC
tags:
- Company
---
