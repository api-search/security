---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flowspecialty.com
  spf: true
hosts:
- host: flowspecialty.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flowspecialty Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flow, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flow
provider_slug: flowspecialty-com
slug: flowspecialty-com-domain-security
source_filename: flowspecialty-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flowspecialty.com\n  https: false\ndomains:\n- domain: flowspecialty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/flowspecialty-com/security/flowspecialty-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
