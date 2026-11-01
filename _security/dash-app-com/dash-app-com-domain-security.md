---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dash-app.com
  spf: true
hosts:
- host: dash-app.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dash App Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dash, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dash
provider_slug: dash-app-com
slug: dash-app-com-domain-security
source_filename: dash-app-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dash-app.com\n  https: false\ndomains:\n- domain: dash-app.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dash-app-com/security/dash-app-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
