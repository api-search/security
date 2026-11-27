---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: good-sport.ai
  spf: true
hosts:
- host: good-sport.ai
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: good-sport-ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for good-sport-ai, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: good-sport-ai
provider_slug: good-sport-ai
slug: good-sport-ai-domain-security
source_filename: good-sport-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: good-sport.ai\n  https: false\ndomains:\n- domain: good-sport.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/good-sport-ai/security/good-sport-ai-domain-security.yml
summary_line: DMARC
tags:
- Company
---
