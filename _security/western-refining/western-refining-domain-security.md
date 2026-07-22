---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: western-refining.com
  spf: true
hosts:
- host: www.western-refining.com
  https: false
kind: domain-security
layout: security
method: probed
name: Western Refining Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for western-refining, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: western-refining
provider_slug: western-refining
slug: western-refining-domain-security
source_filename: western-refining-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.western-refining.com\n  https: false\ndomains:\n- domain: western-refining.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-refining/refs/heads/main/security/western-refining-domain-security.yml
summary_line: DMARC
tags:
- Fortune 500
---
