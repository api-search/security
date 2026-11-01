---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: askenigma.com
  spf: true
hosts:
- host: www.askenigma.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Askenigma Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enigma Analytics, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Enigma Analytics
provider_slug: askenigma-com
slug: askenigma-com-domain-security
source_filename: askenigma-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.askenigma.com\n  https: false\ndomains:\n- domain: askenigma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/askenigma-com/security/askenigma-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
