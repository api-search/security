---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:interlaced@kindred.ai
  dnssec: false
  domain: kindred.ai
  mx:
  - aspmx.l.google.com
  - alt1.aspmx.l.google.com
  - alt2.aspmx.l.google.com
  - alt3.aspmx.l.google.com
  - alt4.aspmx.l.google.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:servers.mcsv.net ?all
hosts: []
kind: domain-security
layout: security
method: probed
name: Kindred Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kindred Ai, probed live across 0 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kindred Ai
provider_slug: kindred-ai
slug: kindred-ai-domain-security
source_filename: kindred-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: dig (kindred.ai) — brand domain; no live developer/web host at time of probe\nnotes: >-\n  kindred.ai resolves to CSC-managed corporate DNS (brand-protection registrar).\n  https://kindred.ai timed out and https://www.kindred.ai returned HTTP 404 at\n  probe time, so there is no live HTTPS web host to record TLS/HSTS for. The\n  registrable domain still carries active Google Workspace mail plus SPF/DMARC,\n  captured below. Absence of a CAA or DNSSEC record is valid recorded data.\nhosts: []\ndomains:\n  - domain: kindred.ai\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: \"v=spf1 include:_spf.google.com include:servers.mcsv.net ?all\"\n    dmarc: true\n    dmarc_policy: none\n    dmarc_record: \"v=DMARC1; p=none; rua=mailto:interlaced@kindred.ai\"\n    mx:\n      - aspmx.l.google.com\n      - alt1.aspmx.l.google.com\n      - alt2.aspmx.l.google.com\n      - alt3.aspmx.l.google.com\n      - alt4.aspmx.l.google.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kindred-ai/refs/heads/main/security/kindred-ai-domain-security.yml
summary_line: DMARC
tags:
- Company
- Robotics
- Artificial Intelligence
- Machine Learning
- Reinforcement Learning
- Warehouse Automation
- Supply Chain
- Acquired
---
