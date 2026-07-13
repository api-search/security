---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dnsforfamily.com
  spf: true
hosts:
- host: corona.dnsforfamily.com
  https: false
kind: domain-security
layout: security
method: probed
name: Graphs For Coronavirus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graphs for Coronavirus, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Graphs for Coronavirus
provider_slug: graphs-for-coronavirus
slug: graphs-for-coronavirus-domain-security
source_filename: graphs-for-coronavirus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corona.dnsforfamily.com\n  https: false\ndomains:\n- domain: dnsforfamily.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphs-for-coronavirus/refs/heads/main/security/graphs-for-coronavirus-domain-security.yml
summary_line: DMARC
tags:
- News
- Public APIs
---
