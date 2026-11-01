---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dejbox.fr
  spf: true
hosts:
- host: www.dejbox.fr
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dejbox Fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dejbox, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dejbox
provider_slug: dejbox-fr
slug: dejbox-fr-domain-security
source_filename: dejbox-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dejbox.fr\n  https: false\ndomains:\n- domain: dejbox.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dejbox-fr/security/dejbox-fr-domain-security.yml
summary_line: DMARC
tags:
- Company
- Cloud Storage
- Document Management
- API Platform
- French Tech
---
