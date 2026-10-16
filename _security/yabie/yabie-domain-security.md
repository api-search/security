---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yabie.com
  spf: true
hosts:
- host: yabie.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yabie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yabie, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yabie
provider_slug: yabie
slug: yabie-domain-security
source_filename: yabie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yabie.com\n  https: false\ndomains:\n- domain: yabie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yabie/refs/heads/main/security/yabie-domain-security.yml
summary_line: DMARC
tags:
- Company
---
