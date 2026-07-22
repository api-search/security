---
description: ''
domains:
- a_records: false
  caa: []
  dmarc: false
  dnssec: false
  domain: pullstring.com
  mx: false
  nameservers:
  - a.ns.apple.com
  - b.ns.apple.com
  - c.ns.apple.com
  - d.ns.apple.com
  spf: true
  spf_record: v=spf1 -all
- a_records: false
  caa: []
  dmarc: false
  dnssec: false
  domain: toytalk.com
  mx: false
  nameservers:
  - a.ns.apple.com
  - b.ns.apple.com
  - c.ns.apple.com
  - d.ns.apple.com
  spf: true
  spf_record: v=spf1 -all
hosts:
- host: pullstring.com
  https: false
- host: toytalk.com
  https: false
kind: domain-security
layout: security
method: probed
name: Toytalk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ToyTalk, probed live across 2 host(s) and 2 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ToyTalk
provider_slug: toytalk
slug: toytalk-domain-security
source_filename: toytalk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnotes: >-\n  Both pullstring.com and toytalk.com are parked domains: no A/AAAA or MX\n  records, delegated to Apple nameservers (a.ns.apple.com - d.ns.apple.com)\n  following Apple's 2019 acquisition of PullString (formerly ToyTalk). The\n  only DNS security posture present is a hard-fail SPF record (v=spf1 -all)\n  on each domain, which prevents mail spoofing from the retired domains.\nhosts:\n- host: pullstring.com\n  https: false\n- host: toytalk.com\n  https: false\ndomains:\n- domain: pullstring.com\n  nameservers: [a.ns.apple.com, b.ns.apple.com, c.ns.apple.com, d.ns.apple.com]\n  a_records: false\n  mx: false\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 -all\n  dmarc: false\n- domain: toytalk.com\n  nameservers: [a.ns.apple.com, b.ns.apple.com, c.ns.apple.com, d.ns.apple.com]\n  a_records: false\n  mx: false\n  dnssec: false\n  caa: []\n  spf: true\n\
  \  spf_record: v=spf1 -all\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toytalk/refs/heads/main/security/toytalk-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Conversational AI
- Voice
- Chatbots
- Entertainment
- Acquired
- Defunct
---
