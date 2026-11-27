---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hardlinephone.com
  spf: false
hosts:
- host: hardlinephone.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: hardlinephone-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hardlinephone-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: hardlinephone-com
provider_slug: hardlinephone-com
slug: hardlinephone-com-domain-security
source_filename: hardlinephone-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hardlinephone.com\n  https: false\ndomains:\n- domain: hardlinephone.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hardlinephone-com/security/hardlinephone-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
