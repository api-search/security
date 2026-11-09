---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bezbaseina.lv
  spf: true
hosts:
- host: bezbaseina.lv
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bezbaseina Lv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bezbaseina-lv, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: bezbaseina-lv
provider_slug: bezbaseina-lv
slug: bezbaseina-lv-domain-security
source_filename: bezbaseina-lv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bezbaseina.lv\n  https: false\ndomains:\n- domain: bezbaseina.lv\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bezbaseina-lv/security/bezbaseina-lv-domain-security.yml
summary_line: DMARC
tags:
- Company
---
