---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: klangoo.com
  spf: true
hosts:
- host: klangoo.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Klangoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klangoo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Klangoo
provider_slug: klangoo
slug: klangoo-domain-security
source_filename: klangoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: klangoo.com\n  https: false\ndomains:\n- domain: klangoo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/klangoo/security/klangoo-domain-security.yml
summary_line: DMARC
tags:
- Company
---
