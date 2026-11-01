---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scripthealth.co
  spf: true
hosts:
- host: scripthealth.co
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scripthealth Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Script Health, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Script Health
provider_slug: scripthealth-co
slug: scripthealth-co-domain-security
source_filename: scripthealth-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scripthealth.co\n  https: false\ndomains:\n- domain: scripthealth.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/scripthealth-co/security/scripthealth-co-domain-security.yml
summary_line: DMARC
tags:
- Company
---
