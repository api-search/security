---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: vboxx.nl
  spf: true
hosts:
- host: vboxx.nl
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vboxx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vBoxx, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: vBoxx
provider_slug: vboxx
slug: vboxx-domain-security
source_filename: vboxx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vboxx.nl\n  https: false\ndomains:\n- domain: vboxx.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/vboxx/security/vboxx-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Cloud
- Infrastructure
- Management
- Security
---
