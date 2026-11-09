---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: djezzy.dz
  spf: true
hosts:
- host: www.djezzy.dz
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Djezzy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Djezzy, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Djezzy
provider_slug: djezzy
slug: djezzy-domain-security
source_filename: djezzy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.djezzy.dz\n  https: false\ndomains:\n- domain: djezzy.dz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/djezzy/security/djezzy-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
---
