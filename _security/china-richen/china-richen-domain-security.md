---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: china-richen.com.cn
  spf: true
hosts:
- host: china-richen.com.cn
  https: false
kind: domain-security
layout: security
method: probed
name: China Richen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for china-richen, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: china-richen
provider_slug: china-richen
slug: china-richen-domain-security
source_filename: china-richen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: china-richen.com.cn\n  https: false\ndomains:\n- domain: china-richen.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/china-richen/refs/heads/main/security/china-richen-domain-security.yml
summary_line: DMARC
tags:
- Company
---
