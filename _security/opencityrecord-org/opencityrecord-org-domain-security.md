---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opencityrecord.org
  spf: true
hosts:
- host: opencityrecord.org
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: opencityrecord-org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for opencityrecord-org, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: opencityrecord-org
provider_slug: opencityrecord-org
slug: opencityrecord-org-domain-security
source_filename: opencityrecord-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencityrecord.org\n  https: false\ndomains:\n- domain: opencityrecord.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/opencityrecord-org/security/opencityrecord-org-domain-security.yml
summary_line: DMARC
tags:
- Company
---
