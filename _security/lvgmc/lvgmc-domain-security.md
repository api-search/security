---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lvgmc.lv
  spf: true
hosts:
- host: lvgmc.lv
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lvgmc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LVGMC (Latvia), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LVGMC (Latvia)
provider_slug: lvgmc
slug: lvgmc-domain-security
source_filename: lvgmc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lvgmc.lv\n  https: false\ndomains:\n- domain: lvgmc.lv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lvgmc/security/lvgmc-domain-security.yml
summary_line: DMARC
tags:
- Company
---
