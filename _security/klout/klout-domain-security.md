---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: klout.com
  spf: false
hosts:
- host: klout.com
  https: false
kind: domain-security
layout: security
method: probed
name: Klout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klout, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Klout
provider_slug: klout
slug: klout-domain-security
source_filename: klout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: klout.com\n  https: false\ndomains:\n- domain: klout.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klout/refs/heads/main/security/klout-domain-security.yml
summary_line: DMARC
tags:
- Company
- Consumer
- Social Media
- Social Analytics
- Influence Scoring
- Social Scoring
- Marketing
- Reputation
- Defunct
- Acquired
---
