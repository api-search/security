---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mitander.io
  spf: true
hosts:
- host: mitander.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: mitander-io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mitander-io, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: mitander-io
provider_slug: mitander-io
slug: mitander-io-domain-security
source_filename: mitander-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mitander.io\n  https: false\ndomains:\n- domain: mitander.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mitander-io/security/mitander-io-domain-security.yml
summary_line: DMARC
tags:
- Company
---
