---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tracedata.io
  spf: true
hosts:
- host: www.tracedata.io
  https: false
kind: domain-security
layout: security
method: probed
name: Trace Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trace Data, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trace Data
provider_slug: trace-data
slug: trace-data-domain-security
source_filename: trace-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tracedata.io\n  https: false\ndomains:\n- domain: tracedata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trace-data/refs/heads/main/security/trace-data-domain-security.yml
summary_line: DMARC
tags:
- Company
- Big Data
- Data Security
- Data Observability
- Data Privacy
- Security
---
