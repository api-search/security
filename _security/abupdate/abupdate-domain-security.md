---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: abupdate.com
  spf: true
hosts:
- host: abupdate.com
  https: false
kind: domain-security
layout: security
method: probed
name: Abupdate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for abupdate, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: abupdate
provider_slug: abupdate
slug: abupdate-domain-security
source_filename: abupdate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abupdate.com\n  https: false\ndomains:\n- domain: abupdate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abupdate/refs/heads/main/security/abupdate-domain-security.yml
summary_line: DMARC
tags:
- Company
---
