---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: actiondesk.io
  spf: true
hosts:
- host: actiondesk.io
  https: false
kind: domain-security
layout: security
method: probed
name: Actiondesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actiondesk, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Actiondesk
provider_slug: actiondesk
slug: actiondesk-domain-security
source_filename: actiondesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: actiondesk.io\n  https: false\ndomains:\n- domain: actiondesk.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actiondesk/refs/heads/main/security/actiondesk-domain-security.yml
summary_line: DMARC
tags:
- Company
---
