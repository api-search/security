---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nugit.ai
  spf: true
hosts:
- host: nugit.ai
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: nugit-ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nugit-ai, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: nugit-ai
provider_slug: nugit-ai
slug: nugit-ai-domain-security
source_filename: nugit-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nugit.ai\n  https: false\ndomains:\n- domain: nugit.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nugit-ai/security/nugit-ai-domain-security.yml
summary_line: DMARC
tags:
- Company
---
