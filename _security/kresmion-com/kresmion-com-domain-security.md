---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kresmion.com
  spf: true
hosts:
- host: kresmion.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: kresmion-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kresmion-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: kresmion-com
provider_slug: kresmion-com
slug: kresmion-com-domain-security
source_filename: kresmion-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kresmion.com\n  https: false\ndomains:\n- domain: kresmion.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kresmion-com/security/kresmion-com-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
---
