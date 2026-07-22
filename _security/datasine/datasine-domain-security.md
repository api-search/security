---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datasine.com
  spf: true
hosts:
- host: datasine.com
  https: false
kind: domain-security
layout: security
method: probed
name: Datasine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataSine, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DataSine
provider_slug: datasine
slug: datasine-domain-security
source_filename: datasine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datasine.com\n  https: false\ndomains:\n- domain: datasine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datasine/refs/heads/main/security/datasine-domain-security.yml
summary_line: DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Personalization
- Marketing
- Acquired
---
