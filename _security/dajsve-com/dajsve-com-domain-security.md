---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dajsve.com
  spf: true
hosts:
- host: dajsve.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dajsve Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dajsve-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: dajsve-com
provider_slug: dajsve-com
slug: dajsve-com-domain-security
source_filename: dajsve-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dajsve.com\n  https: false\ndomains:\n- domain: dajsve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dajsve-com/security/dajsve-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
