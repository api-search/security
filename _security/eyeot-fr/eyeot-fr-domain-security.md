---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: eyeot.fr
  spf: true
hosts:
- host: eyeot.fr
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: eyeot-fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eyeot-fr, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: eyeot-fr
provider_slug: eyeot-fr
slug: eyeot-fr-domain-security
source_filename: eyeot-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eyeot.fr\n  https: false\ndomains:\n- domain: eyeot.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eyeot-fr/security/eyeot-fr-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
---
