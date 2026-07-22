---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: databand.ai
  spf: true
hosts:
- host: databand.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Databand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Databand, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Databand
provider_slug: databand
slug: databand-domain-security
source_filename: databand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: databand.ai\n  https: false\ndomains:\n- domain: databand.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/databand/refs/heads/main/security/databand-domain-security.yml
summary_line: DMARC
tags:
- Company
- Enterprise
- Data Observability
- Data Engineering
- Data Pipelines
- Data Quality
- DataOps
- Machine Learning
- Open Source
- SDK
- CLI
- IBM
---
