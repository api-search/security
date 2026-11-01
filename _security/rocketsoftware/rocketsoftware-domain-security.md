---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rocketsoftware.com
  spf: true
hosts:
- host: rocketsoftware.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rocketsoftware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rocket Software, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rocket Software
provider_slug: rocketsoftware
slug: rocketsoftware-domain-security
source_filename: rocketsoftware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rocketsoftware.com\n  https: false\ndomains:\n- domain: rocketsoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/rocketsoftware/security/rocketsoftware-domain-security.yml
summary_line: DMARC
tags:
- Company
---
