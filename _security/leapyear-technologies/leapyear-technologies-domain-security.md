---
description: ''
domains: []
hosts: []
kind: domain-security
layout: security
method: probed
name: Leapyear Technologies Domain Security
name_suffix: Domain Security
overview: Domain security posture for LeapYear Technologies, probed live across 0 host(s) and 0 registrable domain(s).
provider_name: LeapYear Technologies
provider_slug: leapyear-technologies
slug: leapyear-technologies-domain-security
source_filename: leapyear-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: 0-working/probe-domain-security.py\nprobed: '2026-07-19'\ndomain: leapyear.io\nresult: unreachable\nnotes: >-\n  The probe returned `unreachable` for leapyear.io. HTTPS does not complete a\n  connection (timeout on port 443); only plain HTTP answers, and it serves\n  Snowflake's LeapYear acquisition announcement for every path. The domain is\n  no longer operated as a LeapYear property — it resolves to 3.33.139.32 and is\n  served from MarkMonitor nameservers under Snowflake's control following the\n  February 2023 acquisition. The findings below therefore describe a parked,\n  post-acquisition redirect target, NOT a live LeapYear API edge.\nfindings:\n  tls:\n    available: false\n    detail: HTTPS connection to leapyear.io times out.\n  hsts:\n    present: false\n    detail: Not assessable — no HTTPS response.\n  dnssec:\n    checked: true\n    present: false\n  caa:\n    checked: true\n    records: []\n  spf:\n    checked:\
  \ true\n    records: []\n    detail: No TXT records returned for leapyear.io.\n  dmarc:\n    checked: true\n    records: []\n  mx:\n    checked: true\n    records: []\n    detail: No mail exchangers — the domain no longer receives mail.\ndns:\n  a:\n    - 3.33.139.32\n  nameservers:\n    - ns1.markmonitor.com\n    - ns2.markmonitor.com\n    - ns3.markmonitor.com\n    - ns4.markmonitor.com\n    - ns5.markmonitor.com\n    - ns6.markmonitor.com\n    - ns7.markmonitor.com\n  wildcard: true\n  wildcard_evidence: >-\n    A control request to /this-path-does-not-exist-xyz123 returned 200\n    text/html, identical to /.well-known/security.txt and every other probed\n    path. No /.well-known/ document on this host is genuine.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapyear-technologies/refs/heads/main/security/leapyear-technologies-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Ai Infrastructure
- Differential Privacy
- Data Privacy
- Machine Learning
- Data Clean Rooms
- Privacy Enhancing Technologies
- Acquired
---
