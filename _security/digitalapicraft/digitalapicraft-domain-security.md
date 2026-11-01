---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: digitalapicraft.com
  spf: true
hosts:
- host: digitalapicraft.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Digitalapicraft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DigitalAPI, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DigitalAPI
provider_slug: digitalapicraft
slug: digitalapicraft-domain-security
source_filename: digitalapicraft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digitalapicraft.com\n  https: false\ndomains:\n- domain: digitalapicraft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/digitalapicraft/security/digitalapicraft-domain-security.yml
summary_line: DMARC
tags:
- Company
---
