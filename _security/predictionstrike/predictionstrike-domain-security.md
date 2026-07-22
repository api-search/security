---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: predictionstrike.com
  spf: true
hosts:
- host: www.predictionstrike.com
  https: false
kind: domain-security
layout: security
method: probed
name: Predictionstrike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PredictionStrike, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PredictionStrike
provider_slug: predictionstrike
slug: predictionstrike-domain-security
source_filename: predictionstrike-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.predictionstrike.com\n  https: false\ndomains:\n- domain: predictionstrike.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/predictionstrike/refs/heads/main/security/predictionstrike-domain-security.yml
summary_line: DMARC
tags:
- Company
---
