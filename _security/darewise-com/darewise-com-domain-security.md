---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: darewise.com
  spf: true
hosts:
- host: www.darewise.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Darewise Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Darewise, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Darewise
provider_slug: darewise-com
slug: darewise-com-domain-security
source_filename: darewise-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.darewise.com\n  https: false\ndomains:\n- domain: darewise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/darewise-com/security/darewise-com-domain-security.yml
summary_line: DMARC
tags:
- Company
- Technology
- Startup
- API
- Platform
---
