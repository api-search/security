---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: virushee.com
  spf: true
hosts:
- host: api.virushee.com
  https: false
kind: domain-security
layout: security
method: probed
name: Virushee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virushee, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Virushee
provider_slug: virushee
slug: virushee-domain-security
source_filename: virushee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.virushee.com\n  https: false\ndomains:\n- domain: virushee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virushee/refs/heads/main/security/virushee-domain-security.yml
summary_line: DMARC
tags:
- Security
- Public APIs
---
