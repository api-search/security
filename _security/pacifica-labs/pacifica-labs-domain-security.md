---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thinkpacifica.com
  spf: true
hosts:
- host: thinkpacifica.com
  https: false
kind: domain-security
layout: security
method: probed
name: Pacifica Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pacifica Labs, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pacifica Labs
provider_slug: pacifica-labs
slug: pacifica-labs-domain-security
source_filename: pacifica-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thinkpacifica.com\n  https: false\ndomains:\n- domain: thinkpacifica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pacifica-labs/refs/heads/main/security/pacifica-labs-domain-security.yml
summary_line: DMARC
tags:
- Company
---
